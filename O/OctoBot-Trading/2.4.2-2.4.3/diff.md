# Comparing `tmp/OctoBot-Trading-2.4.2.tar.gz` & `tmp/OctoBot-Trading-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-Trading-2.4.2.tar", last modified: Thu May 11 09:54:59 2023, max compression
+gzip compressed data, was "OctoBot-Trading-2.4.3.tar", last modified: Wed May 17 12:00:17 2023, max compression
```

## Comparing `OctoBot-Trading-2.4.2.tar` & `OctoBot-Trading-2.4.3.tar`

### file list

```diff
@@ -1,573 +1,573 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.462175 OctoBot-Trading-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    32378 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.422176 OctoBot-Trading-2.4.2/OctoBot_Trading.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-11 09:54:59.000000 OctoBot-Trading-2.4.2/OctoBot_Trading.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24325 2023-05-11 09:54:59.000000 OctoBot-Trading-2.4.2/OctoBot_Trading.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:54:59.000000 OctoBot-Trading-2.4.2/OctoBot_Trading.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:54:59.000000 OctoBot-Trading-2.4.2/OctoBot_Trading.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-11 09:54:59.000000 OctoBot-Trading-2.4.2/OctoBot_Trading.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-11 09:54:59.000000 OctoBot-Trading-2.4.2/OctoBot_Trading.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-11 09:54:59.462175 OctoBot-Trading-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.422176 OctoBot-Trading-2.4.2/octobot_trading/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.422176 OctoBot-Trading-2.4.2/octobot_trading/api/
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/api/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/api/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)    11468 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/api/exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/api/modes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/api/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/api/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/api/positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/api/profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/api/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/api/symbol_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/api/trader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/api/trades.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    15028 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.422176 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/
--rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.422176 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/contracts/contract_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/contracts/future_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/contracts/margin_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/exchange_symbol_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/exchange_symbols_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.422176 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/funding/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/funding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.422176 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/funding/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/funding/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/funding/channel/funding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/funding/channel/funding_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/funding/funding_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.422176 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/kline/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/kline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.426175 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/kline/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/kline/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/kline/channel/kline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/kline/channel/kline_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/kline/kline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.426175 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ohlcv/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ohlcv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ohlcv/candles_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ohlcv/candles_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.426175 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ohlcv/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ohlcv/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ohlcv/channel/ohlcv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14894 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.426175 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/order_book/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/order_book/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.426175 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/order_book/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/order_book/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/order_book/channel/order_book.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/order_book/channel/order_book_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/order_book/order_book_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.426175 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/prices/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.426175 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/prices/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/prices/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/prices/channel/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/prices/channel/prices_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/prices/price_events_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/prices/prices_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.426175 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/recent_trades/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/recent_trades/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.426175 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/recent_trades/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/recent_trades/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/recent_trades/channel/recent_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/recent_trades/recent_trades_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.426175 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ticker/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ticker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.426175 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ticker/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ticker/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ticker/channel/ticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ticker/channel/ticker_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ticker/ticker_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.430176 OctoBot-Trading-2.4.2/octobot_trading/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25342 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/abstract_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/abstract_websocket_exchange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.430176 OctoBot-Trading-2.4.2/octobot_trading/exchanges/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/adapters/abstract_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/basic_exchange_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.430176 OctoBot-Trading-2.4.2/octobot_trading/exchanges/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/config/backtesting_exchange_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/config/exchange_config_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.430176 OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.430176 OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/ccxt/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/ccxt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17945 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/ccxt/ccxt_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/ccxt/ccxt_client_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    36361 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/ccxt/ccxt_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    44896 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/ccxt/ccxt_websocket_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/ccxt/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/ccxt/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.430176 OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/simulator/exchange_simulator_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/exchange_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/exchange_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/exchange_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/exchange_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/exchange_websocket_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/exchanges.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.430176 OctoBot-Trading-2.4.2/octobot_trading/exchanges/implementations/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/implementations/default_rest_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/implementations/default_websocket_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/implementations/exchange_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.430176 OctoBot-Trading-2.4.2/octobot_trading/exchanges/traders/
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/traders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42958 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/traders/trader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/traders/trader_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.430176 OctoBot-Trading-2.4.2/octobot_trading/exchanges/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44122 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/types/rest_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/types/websocket_exchange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.430176 OctoBot-Trading-2.4.2/octobot_trading/exchanges/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/util/exchange_market_status_fixer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/util/exchange_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/exchanges/util/websockets_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.430176 OctoBot-Trading-2.4.2/octobot_trading/modes/
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/abstract_trading_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.430176 OctoBot-Trading-2.4.2/octobot_trading/modes/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/channel/abstract_mode_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/channel/abstract_mode_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/channel/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/mode_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/modes_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/modes_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.434176 OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.434176 OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/basic_keywords/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/basic_keywords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/basic_keywords/account_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/basic_keywords/amount.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/basic_keywords/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/basic_keywords/run_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/basic_keywords/trading_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/basic_keywords/user_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25931 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/context_management.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.434176 OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/dsl/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/dsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/dsl/quantity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/dsl/values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.434176 OctoBot-Trading-2.4.2/octobot_trading/modes/scripted_trading_mode/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/scripted_trading_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16335 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/modes/scripted_trading_mode/abstract_scripted_trading_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/octobot_channel_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.434176 OctoBot-Trading-2.4.2/octobot_trading/personal_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19003 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/exchange_personal_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.434176 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.434176 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13853 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/channel/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/channel/orders_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/channel/orders_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/decimal_order_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.434176 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/groups/group_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    41190 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/order.py
--rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/order_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/order_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/order_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    22285 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/order_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/orders_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/orders_storage_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.434176 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/states/
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/states/cancel_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/states/close_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/states/fill_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/states/open_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/states/order_state_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/states/pending_creation_chained_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/states/pending_creation_order_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.434176 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.438176 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/limit/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/limit/buy_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/limit/limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/limit/sell_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/limit/stop_loss_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/limit/take_profit_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.438176 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/market/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/market/buy_market_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/market/market_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/market/sell_market_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.438176 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/trailing/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/trailing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/unknown_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/unsupported_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.438176 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.438176 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/assets/future_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/assets/margin_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/assets/spot_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.438176 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/channel/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/channel/balance_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.438176 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/history/
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/history/historical_asset_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    17826 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14495 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/portfolio_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/portfolio_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/portfolio_profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/portfolio_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/portfolio_value_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/sub_portfolio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.438176 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/types/future_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/types/margin_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/types/spot_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/value_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.442175 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.442175 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/channel/positions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/channel/positions_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/channel/positions_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    38957 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/position_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/position_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/position_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/positions_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.442175 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/states/
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/states/active_position_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/states/idle_position_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/states/liquidate_position_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/states/position_state_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.442175 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/types/inverse_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/types/linear_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.442175 OctoBot-Trading-2.4.2/octobot_trading/personal_data/trades/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/trades/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.442175 OctoBot-Trading-2.4.2/octobot_trading/personal_data/trades/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/trades/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/trades/channel/trades.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/trades/channel/trades_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/trades/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/trades/trade_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/trades/trade_pnl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/trades/trades_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/trades/trades_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.442175 OctoBot-Trading-2.4.2/octobot_trading/personal_data/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/transactions/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/transactions/transaction_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/transactions/transactions_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.442175 OctoBot-Trading-2.4.2/octobot_trading/personal_data/transactions/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/transactions/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/transactions/types/blockchain_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/transactions/types/fee_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/personal_data/transactions/types/transfer_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.442175 OctoBot-Trading-2.4.2/octobot_trading/signals/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/signals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.442175 OctoBot-Trading-2.4.2/octobot_trading/signals/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/signals/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/signals/channel/remote_trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/signals/channel/remote_trading_signal_channel_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/signals/channel/signal_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/signals/signal_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12287 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/signals/trading_signal_bundle_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/signals/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.442175 OctoBot-Trading-2.4.2/octobot_trading/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/storage/abstract_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/storage/candles_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/storage/orders_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/storage/portfolio_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/storage/storage_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/storage/trades_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/storage/transactions_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/storage/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.446175 OctoBot-Trading-2.4.2/octobot_trading/supervisors/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/supervisors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/supervisors/abstract_portfolio_supervisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/supervisors/abstract_supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.446175 OctoBot-Trading-2.4.2/octobot_trading/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/util/config_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/util/initializable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/util/initialization_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/util/simulator_updater_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.446175 OctoBot-Trading-2.4.2/octobot_trading/util/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/util/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/util/test_tools/exchanges_test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/octobot_trading/util/test_tools/websocket_test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 09:54:59.462175 OctoBot-Trading-2.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.418176 OctoBot-Trading-2.4.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.446175 OctoBot-Trading-2.4.2/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/api/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/api/test_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/api/test_modes.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/api/test_orders.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/api/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/api/test_profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/api/test_symbol_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/api/test_trader.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/api/test_trades.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.446175 OctoBot-Trading-2.4.2/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.446175 OctoBot-Trading-2.4.2/tests/exchange_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.446175 OctoBot-Trading-2.4.2/tests/exchange_data/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/contracts/test_future_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/contracts/test_margin_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.446175 OctoBot-Trading-2.4.2/tests/exchange_data/funding/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/funding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/funding/test_funding_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.446175 OctoBot-Trading-2.4.2/tests/exchange_data/kline/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/kline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/kline/test_kline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.446175 OctoBot-Trading-2.4.2/tests/exchange_data/ohlcv/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/ohlcv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/ohlcv/test_candles_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/ohlcv/test_candles_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.446175 OctoBot-Trading-2.4.2/tests/exchange_data/order_book/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/order_book/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/order_book/test_order_book_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.446175 OctoBot-Trading-2.4.2/tests/exchange_data/prices/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/prices/test_price_events_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/prices/test_prices_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.446175 OctoBot-Trading-2.4.2/tests/exchange_data/recent_trades/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/recent_trades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/recent_trades/test_recent_trades_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/test_exchange_symbols_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.446175 OctoBot-Trading-2.4.2/tests/exchange_data/ticker/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/ticker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchange_data/ticker/test_ticker_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.450176 OctoBot-Trading-2.4.2/tests/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.450176 OctoBot-Trading-2.4.2/tests/exchanges/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/connectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.450176 OctoBot-Trading-2.4.2/tests/exchanges/connectors/ccxt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/connectors/ccxt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/connectors/ccxt/test_ccxt_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.450176 OctoBot-Trading-2.4.2/tests/exchanges/implementations/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/implementations/test_default_rest_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/implementations/test_default_websocket_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/test_abstract_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/test_abstract_websocket_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/test_basic_exchange_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/test_exchange_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/test_exchange_config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/test_exchange_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/test_exchange_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/test_exchange_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/test_exchanges.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.450176 OctoBot-Trading-2.4.2/tests/exchanges/traders/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/traders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50864 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/traders/test_trader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.450176 OctoBot-Trading-2.4.2/tests/exchanges/types/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/types/test_websocket_exchange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.450176 OctoBot-Trading-2.4.2/tests/exchanges/util/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/util/test_exchange_market_status_fixer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/exchanges/util/test_exchange_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.450176 OctoBot-Trading-2.4.2/tests/modes/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/modes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.450176 OctoBot-Trading-2.4.2/tests/modes/script_keywords/
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/modes/script_keywords/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.450176 OctoBot-Trading-2.4.2/tests/modes/script_keywords/basic_keywords/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/modes/script_keywords/basic_keywords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/modes/script_keywords/basic_keywords/test_account_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/modes/script_keywords/basic_keywords/test_amount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.450176 OctoBot-Trading-2.4.2/tests/modes/script_keywords/dsl/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/modes/script_keywords/dsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/modes/script_keywords/dsl/test_quantity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/modes/test_abstract_mode_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/modes/test_abstract_trading_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.450176 OctoBot-Trading-2.4.2/tests/personal_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.450176 OctoBot-Trading-2.4.2/tests/personal_data/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.454176 OctoBot-Trading-2.4.2/tests/personal_data/orders/groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19148 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/groups/test_balanced_take_profit_and_stop_order_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/groups/test_group_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/groups/test_one_cancels_the_other_order_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.454176 OctoBot-Trading-2.4.2/tests/personal_data/orders/states/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/states/test_cancel_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/states/test_close_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/states/test_fill_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/states/test_open_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/states/test_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/states/test_order_state_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/states/test_pending_creation_chained_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/states/test_pending_creation_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/test_decimal_order_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/test_double_filled_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    18703 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/test_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    20330 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/test_order_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/test_order_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    25593 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/test_order_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/test_orders_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/test_orders_storage_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.454176 OctoBot-Trading-2.4.2/tests/personal_data/orders/types/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.454176 OctoBot-Trading-2.4.2/tests/personal_data/orders/types/limit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/types/limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/types/limit/test_buy_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/types/limit/test_sell_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/types/limit/test_stop_loss_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/types/limit/test_take_profit_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/types/limit/test_take_profit_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.454176 OctoBot-Trading-2.4.2/tests/personal_data/orders/types/market/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/types/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/types/market/test_buy_market_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/types/market/test_sell_market_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/types/test_unknown_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.454176 OctoBot-Trading-2.4.2/tests/personal_data/orders/types/trailing/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/types/trailing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/types/trailing/test_trailing_stop_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/orders/types/trailing/test_trailing_stop_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.454176 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.454176 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/assets/test_future_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/assets/test_margin_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/assets/test_spot_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.454176 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/history/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/history/test_historical_asset_value_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    31055 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/history/test_historical_portfolio_value_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/test_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    52120 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/test_portfolio_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/test_portfolio_profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)    11149 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/test_portfolio_value_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/test_value_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.458176 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/types/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85551 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/types/test_future_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/types/test_margin_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/portfolios/types/test_spot_portfolio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.458176 OctoBot-Trading-2.4.2/tests/personal_data/positions/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/positions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.458176 OctoBot-Trading-2.4.2/tests/personal_data/positions/channel/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/positions/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.458176 OctoBot-Trading-2.4.2/tests/personal_data/positions/states/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/positions/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67901 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/positions/test_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/positions/test_position_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/positions/test_positions_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.458176 OctoBot-Trading-2.4.2/tests/personal_data/positions/types/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/positions/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/positions/types/test_inverse_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    45257 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/positions/types/test_linear_position.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.458176 OctoBot-Trading-2.4.2/tests/personal_data/trades/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/trades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/trades/test_trade_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/trades/test_trade_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/trades/test_trade_pnl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.458176 OctoBot-Trading-2.4.2/tests/personal_data/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/transactions/test_transaction_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/personal_data/transactions/test_transactions_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.458176 OctoBot-Trading-2.4.2/tests/signals/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30314 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/signals/test_trading_signal_bundle_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/signals/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.458176 OctoBot-Trading-2.4.2/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/test_utils/order_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/test_utils/random_numbers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.458176 OctoBot-Trading-2.4.2/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests/util/test_config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.458176 OctoBot-Trading-2.4.2/tests_additional/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:54:59.462175 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/real_exchange_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/real_futures_exchange_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_ascendex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_binance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_bitfinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_bitget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_bithumb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_bitso.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_bitstamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_bittrex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_bybit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_bybit_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_coinbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_coinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_cryptocom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_gateio.py
--rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_hitbtc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_hollaex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_huobi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_huobipro.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_kraken.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_kucoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_kucoin_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_ndax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_okcoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_okx.py
--rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_okx_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_phemex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_poloniex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_upbit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-05-11 09:54:04.000000 OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_wavesexchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.229746 OctoBot-Trading-2.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    32492 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.181745 OctoBot-Trading-2.4.3/OctoBot_Trading.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-17 12:00:17.000000 OctoBot-Trading-2.4.3/OctoBot_Trading.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24325 2023-05-17 12:00:17.000000 OctoBot-Trading-2.4.3/OctoBot_Trading.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:00:17.000000 OctoBot-Trading-2.4.3/OctoBot_Trading.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:00:17.000000 OctoBot-Trading-2.4.3/OctoBot_Trading.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-17 12:00:17.000000 OctoBot-Trading-2.4.3/OctoBot_Trading.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-17 12:00:17.000000 OctoBot-Trading-2.4.3/OctoBot_Trading.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-17 12:00:17.225746 OctoBot-Trading-2.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.185746 OctoBot-Trading-2.4.3/octobot_trading/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.185746 OctoBot-Trading-2.4.3/octobot_trading/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/api/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/api/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11468 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/api/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/api/modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/api/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/api/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/api/positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/api/profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/api/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/api/symbol_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/api/trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/api/trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.185746 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.185746 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/contracts/contract_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/contracts/future_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/contracts/margin_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/exchange_symbol_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/exchange_symbols_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.185746 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/funding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/funding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.185746 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/funding/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/funding/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/funding/channel/funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/funding/channel/funding_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/funding/funding_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.185746 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/kline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/kline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.185746 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/kline/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/kline/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/kline/channel/kline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/kline/channel/kline_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/kline/kline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.185746 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ohlcv/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ohlcv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ohlcv/candles_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ohlcv/candles_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.189746 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ohlcv/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ohlcv/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ohlcv/channel/ohlcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.189746 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/order_book/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/order_book/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.189746 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/order_book/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/order_book/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/order_book/channel/order_book.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/order_book/channel/order_book_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/order_book/order_book_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.189746 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/prices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.189746 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/prices/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/prices/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/prices/channel/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/prices/channel/prices_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/prices/price_events_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/prices/prices_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.189746 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/recent_trades/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/recent_trades/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.189746 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/recent_trades/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/recent_trades/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/recent_trades/channel/recent_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/recent_trades/recent_trades_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.189746 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ticker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ticker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.189746 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ticker/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ticker/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ticker/channel/ticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ticker/channel/ticker_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ticker/ticker_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.189746 OctoBot-Trading-2.4.3/octobot_trading/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25402 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/abstract_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/abstract_websocket_exchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.189746 OctoBot-Trading-2.4.3/octobot_trading/exchanges/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/adapters/abstract_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/basic_exchange_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.193746 OctoBot-Trading-2.4.3/octobot_trading/exchanges/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/config/backtesting_exchange_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/config/exchange_config_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.193746 OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.193746 OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/ccxt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/ccxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18004 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/ccxt/ccxt_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/ccxt/ccxt_client_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/ccxt/ccxt_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44896 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/ccxt/ccxt_websocket_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/ccxt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/ccxt/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.193746 OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/simulator/exchange_simulator_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/exchange_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/exchange_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/exchange_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/exchange_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/exchange_websocket_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/exchanges.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.193746 OctoBot-Trading-2.4.3/octobot_trading/exchanges/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/implementations/default_rest_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/implementations/default_websocket_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/implementations/exchange_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.193746 OctoBot-Trading-2.4.3/octobot_trading/exchanges/traders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/traders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42921 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/traders/trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/traders/trader_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.193746 OctoBot-Trading-2.4.3/octobot_trading/exchanges/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44555 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/types/rest_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/types/websocket_exchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.193746 OctoBot-Trading-2.4.3/octobot_trading/exchanges/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/util/exchange_market_status_fixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14753 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/util/exchange_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/exchanges/util/websockets_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.193746 OctoBot-Trading-2.4.3/octobot_trading/modes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/abstract_trading_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.193746 OctoBot-Trading-2.4.3/octobot_trading/modes/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/channel/abstract_mode_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/channel/abstract_mode_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/channel/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/mode_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/modes_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/modes_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.193746 OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.197746 OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/basic_keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/basic_keywords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/basic_keywords/account_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/basic_keywords/amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/basic_keywords/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/basic_keywords/run_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/basic_keywords/trading_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/basic_keywords/user_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25931 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/context_management.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.197746 OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/dsl/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/dsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/dsl/quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/dsl/values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.197746 OctoBot-Trading-2.4.3/octobot_trading/modes/scripted_trading_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/scripted_trading_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16335 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/modes/scripted_trading_mode/abstract_scripted_trading_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/octobot_channel_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.197746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19216 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/exchange_personal_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.197746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.197746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/channel/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/channel/orders_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/channel/orders_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/decimal_order_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.197746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/groups/group_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41048 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/order_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/order_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/order_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22239 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/order_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/orders_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/orders_storage_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.197746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/states/
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/states/cancel_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/states/close_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/states/fill_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/states/open_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/states/order_state_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/states/pending_creation_chained_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/states/pending_creation_order_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.201746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.201746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/limit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/limit/buy_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/limit/limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/limit/sell_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/limit/stop_loss_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/limit/take_profit_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.201746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/market/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/market/buy_market_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/market/market_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/market/sell_market_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.201746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/trailing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/trailing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/unknown_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/unsupported_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.201746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.201746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/assets/future_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/assets/margin_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/assets/spot_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.201746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/channel/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/channel/balance_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.201746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/history/
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/history/historical_asset_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17826 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14495 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/portfolio_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/portfolio_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/portfolio_profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/portfolio_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/portfolio_value_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/sub_portfolio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.205746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/types/future_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/types/margin_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/types/spot_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/value_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.205746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.205746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/channel/positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/channel/positions_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/channel/positions_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38957 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/position_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/position_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/position_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/positions_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.205746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/states/
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/states/active_position_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/states/idle_position_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/states/liquidate_position_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/states/position_state_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.205746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/types/inverse_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/types/linear_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.205746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/trades/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/trades/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.205746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/trades/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/trades/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/trades/channel/trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/trades/channel/trades_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/trades/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/trades/trade_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/trades/trade_pnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/trades/trades_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/trades/trades_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.205746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/transactions/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/transactions/transaction_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/transactions/transactions_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.205746 OctoBot-Trading-2.4.3/octobot_trading/personal_data/transactions/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/transactions/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/transactions/types/blockchain_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/transactions/types/fee_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/personal_data/transactions/types/transfer_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.205746 OctoBot-Trading-2.4.3/octobot_trading/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/signals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.209746 OctoBot-Trading-2.4.3/octobot_trading/signals/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/signals/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/signals/channel/remote_trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/signals/channel/remote_trading_signal_channel_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/signals/channel/signal_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/signals/signal_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/signals/trading_signal_bundle_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/signals/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.209746 OctoBot-Trading-2.4.3/octobot_trading/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/storage/abstract_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/storage/candles_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/storage/orders_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/storage/portfolio_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/storage/storage_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/storage/trades_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/storage/transactions_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/storage/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.209746 OctoBot-Trading-2.4.3/octobot_trading/supervisors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/supervisors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/supervisors/abstract_portfolio_supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/supervisors/abstract_supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.209746 OctoBot-Trading-2.4.3/octobot_trading/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/util/config_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/util/initializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/util/initialization_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/util/simulator_updater_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.209746 OctoBot-Trading-2.4.3/octobot_trading/util/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/util/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/util/test_tools/exchanges_test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/octobot_trading/util/test_tools/websocket_test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:00:17.229746 OctoBot-Trading-2.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.181745 OctoBot-Trading-2.4.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.209746 OctoBot-Trading-2.4.3/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/api/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/api/test_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/api/test_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/api/test_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/api/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/api/test_profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/api/test_symbol_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/api/test_trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/api/test_trades.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.209746 OctoBot-Trading-2.4.3/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.209746 OctoBot-Trading-2.4.3/tests/exchange_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.209746 OctoBot-Trading-2.4.3/tests/exchange_data/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/contracts/test_future_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/contracts/test_margin_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.209746 OctoBot-Trading-2.4.3/tests/exchange_data/funding/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/funding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/funding/test_funding_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.213746 OctoBot-Trading-2.4.3/tests/exchange_data/kline/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/kline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/kline/test_kline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.213746 OctoBot-Trading-2.4.3/tests/exchange_data/ohlcv/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/ohlcv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/ohlcv/test_candles_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/ohlcv/test_candles_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.213746 OctoBot-Trading-2.4.3/tests/exchange_data/order_book/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/order_book/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/order_book/test_order_book_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.213746 OctoBot-Trading-2.4.3/tests/exchange_data/prices/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/prices/test_price_events_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/prices/test_prices_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.213746 OctoBot-Trading-2.4.3/tests/exchange_data/recent_trades/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/recent_trades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/recent_trades/test_recent_trades_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/test_exchange_symbols_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.213746 OctoBot-Trading-2.4.3/tests/exchange_data/ticker/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/ticker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchange_data/ticker/test_ticker_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.213746 OctoBot-Trading-2.4.3/tests/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.213746 OctoBot-Trading-2.4.3/tests/exchanges/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/connectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.213746 OctoBot-Trading-2.4.3/tests/exchanges/connectors/ccxt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/connectors/ccxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/connectors/ccxt/test_ccxt_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.213746 OctoBot-Trading-2.4.3/tests/exchanges/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/implementations/test_default_rest_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/implementations/test_default_websocket_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/test_abstract_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/test_abstract_websocket_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/test_basic_exchange_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/test_exchange_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/test_exchange_config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/test_exchange_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/test_exchange_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/test_exchange_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/test_exchanges.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.213746 OctoBot-Trading-2.4.3/tests/exchanges/traders/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/traders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50864 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/traders/test_trader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.213746 OctoBot-Trading-2.4.3/tests/exchanges/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/types/test_websocket_exchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.213746 OctoBot-Trading-2.4.3/tests/exchanges/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/util/test_exchange_market_status_fixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/exchanges/util/test_exchange_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.213746 OctoBot-Trading-2.4.3/tests/modes/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/modes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.213746 OctoBot-Trading-2.4.3/tests/modes/script_keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/modes/script_keywords/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.217746 OctoBot-Trading-2.4.3/tests/modes/script_keywords/basic_keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/modes/script_keywords/basic_keywords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/modes/script_keywords/basic_keywords/test_account_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/modes/script_keywords/basic_keywords/test_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.217746 OctoBot-Trading-2.4.3/tests/modes/script_keywords/dsl/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/modes/script_keywords/dsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/modes/script_keywords/dsl/test_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/modes/test_abstract_mode_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/modes/test_abstract_trading_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.217746 OctoBot-Trading-2.4.3/tests/personal_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.217746 OctoBot-Trading-2.4.3/tests/personal_data/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.217746 OctoBot-Trading-2.4.3/tests/personal_data/orders/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19148 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/groups/test_balanced_take_profit_and_stop_order_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/groups/test_group_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/groups/test_one_cancels_the_other_order_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.217746 OctoBot-Trading-2.4.3/tests/personal_data/orders/states/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/states/test_cancel_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/states/test_close_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/states/test_fill_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/states/test_open_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/states/test_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/states/test_order_state_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/states/test_pending_creation_chained_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/states/test_pending_creation_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/test_decimal_order_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/test_double_filled_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19279 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/test_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20330 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/test_order_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/test_order_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25593 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/test_order_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/test_orders_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/test_orders_storage_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.217746 OctoBot-Trading-2.4.3/tests/personal_data/orders/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.217746 OctoBot-Trading-2.4.3/tests/personal_data/orders/types/limit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/types/limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/types/limit/test_buy_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/types/limit/test_sell_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/types/limit/test_stop_loss_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/types/limit/test_take_profit_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/types/limit/test_take_profit_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.217746 OctoBot-Trading-2.4.3/tests/personal_data/orders/types/market/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/types/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/types/market/test_buy_market_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/types/market/test_sell_market_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/types/test_unknown_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.221746 OctoBot-Trading-2.4.3/tests/personal_data/orders/types/trailing/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/types/trailing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/types/trailing/test_trailing_stop_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/orders/types/trailing/test_trailing_stop_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.221746 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.221746 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/assets/test_future_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/assets/test_margin_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/assets/test_spot_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.221746 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/history/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/history/test_historical_asset_value_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31055 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/history/test_historical_portfolio_value_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/test_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52120 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/test_portfolio_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/test_portfolio_profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11149 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/test_portfolio_value_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/test_value_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.221746 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85551 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/types/test_future_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/types/test_margin_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/portfolios/types/test_spot_portfolio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.221746 OctoBot-Trading-2.4.3/tests/personal_data/positions/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/positions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.221746 OctoBot-Trading-2.4.3/tests/personal_data/positions/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/positions/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.221746 OctoBot-Trading-2.4.3/tests/personal_data/positions/states/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/positions/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67901 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/positions/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/positions/test_position_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/positions/test_positions_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.221746 OctoBot-Trading-2.4.3/tests/personal_data/positions/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/positions/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/positions/types/test_inverse_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45257 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/positions/types/test_linear_position.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.221746 OctoBot-Trading-2.4.3/tests/personal_data/trades/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/trades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/trades/test_trade_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/trades/test_trade_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/trades/test_trade_pnl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.221746 OctoBot-Trading-2.4.3/tests/personal_data/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/transactions/test_transaction_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/personal_data/transactions/test_transactions_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.221746 OctoBot-Trading-2.4.3/tests/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29924 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/signals/test_trading_signal_bundle_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/signals/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.225746 OctoBot-Trading-2.4.3/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/test_utils/order_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/test_utils/random_numbers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.225746 OctoBot-Trading-2.4.3/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests/util/test_config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.225746 OctoBot-Trading-2.4.3/tests_additional/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:17.225746 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/real_exchange_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/real_futures_exchange_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_ascendex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_bitfinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_bitget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_bithumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_bitso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_bitstamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_bittrex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_bybit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_bybit_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_coinbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_coinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_cryptocom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_gateio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_hitbtc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_hollaex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_huobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_huobipro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_kraken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_kucoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_kucoin_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_ndax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_okcoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_okx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_okx_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_phemex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_poloniex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_upbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-05-17 11:59:24.000000 OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_wavesexchange.py
```

### Comparing `OctoBot-Trading-2.4.2/CHANGELOG.md` & `OctoBot-Trading-2.4.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.4.3] - 2023-05-12
+### Updated
+- Use orders shared if for pnl
+### Fixed
+- Chained orders in trading signals
+
 ## [2.4.2] - 2023-05-10
 ### Added
 - Display timeframe
 - Quote denominated amount in trading modes settings
 ### Updated
 - Orders API
 ### Fixed
```

### Comparing `OctoBot-Trading-2.4.2/LICENSE` & `OctoBot-Trading-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/OctoBot_Trading.egg-info/PKG-INFO` & `OctoBot-Trading-2.4.3/OctoBot_Trading.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Trading
-Version: 2.4.2
+Version: 2.4.3
 Summary: OctoBot project trading package
 Home-page: https://github.com/Drakkar-Software/OctoBot-Trading
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# OctoBot-Trading [2.4.2](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
+# OctoBot-Trading [2.4.3](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/903b6b22bceb4661b608a86fea655f69)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Trading?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Trading&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Trading.svg)](https://pypi.python.org/pypi/OctoBot-Trading/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Trading/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Trading?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Trading/workflows/OctoBot-Trading-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Trading/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Trading/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Trading)
 
 OctoBot trading package.
```

### Comparing `OctoBot-Trading-2.4.2/OctoBot_Trading.egg-info/SOURCES.txt` & `OctoBot-Trading-2.4.3/OctoBot_Trading.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/PKG-INFO` & `OctoBot-Trading-2.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Trading
-Version: 2.4.2
+Version: 2.4.3
 Summary: OctoBot project trading package
 Home-page: https://github.com/Drakkar-Software/OctoBot-Trading
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# OctoBot-Trading [2.4.2](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
+# OctoBot-Trading [2.4.3](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/903b6b22bceb4661b608a86fea655f69)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Trading?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Trading&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Trading.svg)](https://pypi.python.org/pypi/OctoBot-Trading/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Trading/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Trading?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Trading/workflows/OctoBot-Trading-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Trading/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Trading/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Trading)
 
 OctoBot trading package.
```

### Comparing `OctoBot-Trading-2.4.2/README.md` & `OctoBot-Trading-2.4.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OctoBot-Trading [2.4.2](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
+# OctoBot-Trading [2.4.3](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/903b6b22bceb4661b608a86fea655f69)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Trading?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Trading&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Trading.svg)](https://pypi.python.org/pypi/OctoBot-Trading/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Trading/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Trading?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Trading/workflows/OctoBot-Trading-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Trading/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Trading/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Trading)
 
 OctoBot trading package.
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
 PROJECT_NAME = "OctoBot-Trading"
-VERSION = "2.4.2"  # major.minor.revision
+VERSION = "2.4.3"  # major.minor.revision
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/api/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/api/channels.py` & `OctoBot-Trading-2.4.3/octobot_trading/api/channels.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/api/contracts.py` & `OctoBot-Trading-2.4.3/octobot_trading/api/contracts.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/api/exchange.py` & `OctoBot-Trading-2.4.3/octobot_trading/api/exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/api/modes.py` & `OctoBot-Trading-2.4.3/octobot_trading/api/modes.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/api/orders.py` & `OctoBot-Trading-2.4.3/octobot_trading/api/orders.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/api/portfolio.py` & `OctoBot-Trading-2.4.3/octobot_trading/api/portfolio.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,22 +36,20 @@
     return []
 
 
 def get_global_portfolio_currencies_values(exchange_managers: list) -> dict:
     currencies_values = {}
     for exchange in exchange_managers:
         this_currency_values = (
-            exchange.exchange_personal_data.portfolio_manager \
-                .portfolio_value_holder.get_current_crypto_currencies_values()
+            exchange.exchange_personal_data.portfolio_manager
+            .portfolio_value_holder.get_current_crypto_currencies_values()
         )
         for currency, value in this_currency_values.items():
             if currency not in currencies_values:
                 currencies_values[currency] = value
-            else:
-                currencies_values[currency] += value
     return currencies_values
 
 
 def get_portfolio_currency(exchange_manager, currency) -> personal_data.Asset:
     return exchange_manager.exchange_personal_data.portfolio_manager.portfolio.get_currency_portfolio(currency)
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/api/positions.py` & `OctoBot-Trading-2.4.3/octobot_trading/api/positions.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/api/profitability.py` & `OctoBot-Trading-2.4.3/octobot_trading/api/profitability.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/api/storage.py` & `OctoBot-Trading-2.4.3/octobot_trading/api/storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/api/symbol_data.py` & `OctoBot-Trading-2.4.3/octobot_trading/api/symbol_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/api/trader.py` & `OctoBot-Trading-2.4.3/octobot_trading/api/trader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/api/trades.py` & `OctoBot-Trading-2.4.3/octobot_trading/api/trades.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 def get_trade_history(
         exchange_manager, quote=None, symbol=None, since=None, as_dict=False, include_cancelled=False
 ) -> list:
     return [
         trade.to_dict() if as_dict else trade
-        for trade in exchange_manager.exchange_personal_data.trades_manager.trades.values()
+        for trade in exchange_manager.exchange_personal_data.trades_manager.get_trades()
         if _trade_filter(trade, quote, symbol, since, include_cancelled)
     ]
 
 
 def get_completed_pnl_history(exchange_manager, quote=None, symbol=None, since=None) -> list:
     return exchange_manager.exchange_personal_data.trades_manager.get_completed_trades_pnl(
         get_trade_history(
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/constants.py` & `OctoBot-Trading-2.4.3/octobot_trading/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -177,24 +177,14 @@
                            enums.OrderStatus.FILLED,
                            enums.OrderStatus.PARTIALLY_FILLED]
 CANCEL_ORDER_STATUS_SCOPE = [enums.OrderStatus.PENDING_CANCEL,
                              enums.OrderStatus.CANCELED,
                              enums.OrderStatus.EXPIRED,
                              enums.OrderStatus.REJECTED]
 
-ORDER_NON_EMPTY_FIELDS = [enums.ExchangeConstantsOrderColumns.ID.value,
-                          enums.ExchangeConstantsOrderColumns.TIMESTAMP.value,
-                          enums.ExchangeConstantsOrderColumns.SYMBOL.value,
-                          enums.ExchangeConstantsOrderColumns.TYPE.value,
-                          enums.ExchangeConstantsOrderColumns.SIDE.value,
-                          enums.ExchangeConstantsOrderColumns.PRICE.value,
-                          enums.ExchangeConstantsOrderColumns.AMOUNT.value,
-                          enums.ExchangeConstantsOrderColumns.STATUS.value]
-ORDER_REQUIRED_FIELDS = ORDER_NON_EMPTY_FIELDS + [enums.ExchangeConstantsOrderColumns.REMAINING.value]
-
 DEFAULT_INITIALIZATION_EVENT_TOPICS = [
     commons_enums.InitializationEventExchangeTopics.BALANCE,
     commons_enums.InitializationEventExchangeTopics.ORDERS,
     commons_enums.InitializationEventExchangeTopics.TRADES,
     commons_enums.InitializationEventExchangeTopics.CANDLES,
     commons_enums.InitializationEventExchangeTopics.PRICE,
 ]
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/enums.py` & `OctoBot-Trading-2.4.3/octobot_trading/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,14 +295,15 @@
     SYMBOL = "symbol"
     TIMESTAMP = "timestamp"
 
 
 class ExchangeConstantsOrderColumns(enum.Enum):
     INFO = "info"
     ID = "id"
+    EXCHANGE_ID = "exchange_id"
     ORDER_ID = "order_id"
     TIMESTAMP = "timestamp"
     DATETIME = 'datetime'
     LAST_TRADE_TIMESTAMP = "lastTradeTimestamp"
     SYMBOL = "symbol"
     MARKET = "market"
     QUANTITY_CURRENCY = "quantity_currency"
@@ -327,14 +328,18 @@
     TAKE_PROFIT_PRICE = "takeProfitPrice"
     TRIGGER_ABOVE = "triggerAbove"
     TAG = "tag"
     SELF_MANAGED = "self-managed"
     ENTRIES = "entries"
 
 
+class TradeExtraConstants(enum.Enum):
+    CREATION_TIME = "creation_time"
+
+
 class ExchangeConstantsPositionColumns(enum.Enum):
     ID = "id"
     TIMESTAMP = "timestamp"
     SYMBOL = "symbol"
     ENTRY_PRICE = "entry_price"
     MARK_PRICE = "mark_price"
     LIQUIDATION_PRICE = "liquidation_price"
@@ -519,15 +524,15 @@
     CURRENT_PRICE = "current"
     UPDATED_CURRENT_PRICE = "updated_current_price"
     REDUCE_ONLY = "reduce_only"
     POST_ONLY = "post_only"
     GROUP_ID = "group_id"
     GROUP_TYPE = "group_type"
     TAG = "tag"
-    SHARED_SIGNAL_ORDER_ID = "shared_signal_order_id"
+    ORDER_ID = "order_id"
     BUNDLED_WITH = "bundled_with"
     CHAINED_TO = "chained_to"
     ADDITIONAL_ORDERS = "additional_orders"
     ASSOCIATED_ORDER_IDS = "associated_order_ids"
     UPDATE_WITH_TRIGGERING_ORDER_FEES = "update_with_triggering_order_fees"
 
 
@@ -541,20 +546,20 @@
 class StoredOrdersAttr(enum.Enum):
     GROUP = "gr"
     GROUP_ID = "gi"
     GROUP_TYPE = "gt"
     CHAINED_ORDERS = "co"
     EXCHANGE_CREATION_PARAMS = "ecp"
     TRADER_CREATION_KWARGS = "tck"
-    SHARED_SIGNAL_ORDER_ID = "ssoi"
     HAS_BEEN_BUNDLED = "hbb"
     ENTRIES = "en"
     UPDATE_TIME = "ut"
     UPDATE_TYPE = "uty"
     ORDER_ID = "oid"
+    ORDER_EXCHANGE_ID = "oeid"
     ORDER_STATUS = "s"
     ORDER_DETAILS = "d"
     UPDATE_WITH_TRIGGERING_ORDER_FEES = "utf"
 
 
 class OrderUpdateType(enum.Enum):
     NEW = "new"
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/errors.py` & `OctoBot-Trading-2.4.3/octobot_trading/errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -107,24 +107,14 @@
 
 class PortfolioOperationError(Exception):
     """
     Raised when an invalid portfolio operation is asked for
     """
 
 
-class MissingOrderException(Exception):
-    """
-    Raised when an order is missing
-    """
-
-    def __init__(self, order_id):
-        super().__init__()
-        self.order_id = order_id
-
-
 class InvalidOrderState(Exception):
     """
     Raised when an order state is handled on a previously cleared order
     (cleared orders should never be touched)
     """
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_channel.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_channel.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/contracts/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/contracts/contract_factory.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/contracts/contract_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/contracts/future_contract.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/contracts/future_contract.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/contracts/margin_contract.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/contracts/margin_contract.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/exchange_symbol_data.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/exchange_symbol_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/exchange_symbols_data.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/exchange_symbols_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/funding/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/funding/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/funding/channel/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/funding/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/funding/channel/funding.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/funding/channel/funding.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/funding/channel/funding_updater.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/funding/channel/funding_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/funding/funding_manager.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/funding/funding_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/kline/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/kline/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/kline/channel/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/kline/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/kline/channel/kline.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/kline/channel/kline.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/kline/channel/kline_updater.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/kline/channel/kline_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/kline/kline_manager.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/kline/kline_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ohlcv/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ohlcv/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ohlcv/candles_adapter.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ohlcv/candles_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ohlcv/candles_manager.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ohlcv/candles_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ohlcv/channel/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ohlcv/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ohlcv/channel/ohlcv.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ohlcv/channel/ohlcv.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
                     asyncio.create_task(self._candle_update_loop(time_frame, pair))
                     for time_frame in self._get_time_frames()
                     for pair in self._get_traded_pairs()
                     if self._should_maintain_candle(time_frame, pair)
                 ]
 
     def _get_traded_pairs(self):
-        return self.channel.exchange_manager.exchange_config.watched_pairs
+        return self.channel.exchange_manager.exchange_config.traded_symbol_pairs
 
     def _get_time_frames(self):
         return self.channel.exchange_manager.exchange_config.available_time_frames
 
     def _should_maintain_candle(self, time_frame, pair):
         return not (
             exchanges.is_channel_managed_by_websocket(self.channel.exchange_manager, self.CHANNEL_NAME)
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/order_book/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/order_book/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/order_book/channel/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/order_book/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/order_book/channel/order_book.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/order_book/channel/order_book.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/order_book/channel/order_book_updater.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/order_book/channel/order_book_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/order_book/order_book_manager.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/order_book/order_book_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/prices/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/prices/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/prices/channel/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/prices/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/prices/channel/price.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/prices/channel/price.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/prices/channel/prices_updater.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/prices/channel/prices_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/prices/price_events_manager.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/prices/price_events_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/prices/prices_manager.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/prices/prices_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/recent_trades/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/recent_trades/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/recent_trades/channel/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/recent_trades/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/recent_trades/channel/recent_trade.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/recent_trades/channel/recent_trade.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/recent_trades/recent_trades_manager.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/recent_trades/recent_trades_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ticker/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ticker/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ticker/channel/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ticker/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ticker/channel/ticker.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ticker/channel/ticker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ticker/channel/ticker_updater.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ticker/channel/ticker_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchange_data/ticker/ticker_manager.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchange_data/ticker/ticker_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/abstract_exchange.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/abstract_exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,18 +223,18 @@
     async def get_all_currencies_price_ticker(self, **kwargs: dict) -> typing.Optional[list]:
         """
         Get all exchange currency tickers
         :return: the list of exchange currencies tickers
         """
         raise NotImplementedError("get_all_currencies_price_ticker is not implemented")
 
-    async def get_order(self, order_id: str, symbol: str = None, **kwargs: dict) -> dict:
+    async def get_order(self, exchange_order_id: str, symbol: str = None, **kwargs: dict) -> dict:
         """
         Get the order data from the exchange
-        :param order_id: the order id
+        :param exchange_order_id: the order id on exchange
         :param symbol: the order symbol
         :return: the order data
         """
         raise NotImplementedError("get_order is not implemented")
 
     async def get_all_orders(self, symbol: str = None, since: int = None,
                              limit: int = None, **kwargs: dict) -> list:
@@ -284,19 +284,19 @@
         """
         :param symbols: the symbols or None
         :return: the current leverage tiers by symbols
         """
         raise NotImplementedError("get_leverage_tiers is not implemented")
 
     async def cancel_order(
-            self, order_id: str, symbol: str, order_type: enums.TraderOrderType, **kwargs: dict
+            self, exchange_order_id: str, symbol: str, order_type: enums.TraderOrderType, **kwargs: dict
     ) -> enums.OrderStatus:
         """
         Cancel a order on the exchange
-        :param order_id: the order id
+        :param exchange_order_id: the order id on exchange
         :param symbol: the order symbol
         :param order_type: the type of the order
         :return: True if the order is successfully cancelled
         """
         raise NotImplementedError("cancel_order is not implemented")
 
     async def create_order(self, order_type: enums.TraderOrderType, symbol: str, quantity: decimal.Decimal,
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/abstract_websocket_exchange.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/abstract_websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/adapters/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/adapters/abstract_adapter.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/adapters/abstract_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import decimal
 
 import octobot_trading.errors as errors
+import octobot_trading.enums as enums
 import octobot_commons.logging as logging
 import octobot_commons.constants as commons_constants
 
 
 def _adapter(func):
     def wrapper(*args, **kwargs):
         try:
@@ -129,14 +130,17 @@
 
     def safe_decimal(self, container, key, default):
         if (val := container.get(key, default)) is not None:
             return decimal.Decimal(str(val))
         return default
 
     def fix_order(self, raw, **kwargs):
+        # id is reserved for octobot managed id. store exchange id in EXCHANGE_ID
+        raw[enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value] = \
+            raw.pop(enums.ExchangeConstantsOrderColumns.ID.value, None)
         # add generic logic if necessary
         return raw
 
     def parse_order(self, fixed, **kwargs):
         raise NotImplementedError("parse_order is not implemented")
 
     def fix_ohlcv(self, raw, **kwargs):
@@ -178,15 +182,19 @@
         # add generic logic if necessary
         return raw
 
     def parse_public_recent_trades(self, fixed, **kwargs):
         raise NotImplementedError("parse_public_recent_trades is not implemented")
 
     def fix_trades(self, raw, **kwargs):
-        # add generic logic if necessary
+        for trade in raw:
+            # id is reserved for octobot managed id. store exchange id in EXCHANGE_ID
+            trade[enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value] = \
+                trade.pop(enums.ExchangeConstantsOrderColumns.ID.value, None)
+            # add generic logic if necessary
         return raw
 
     def parse_trades(self, fixed, **kwargs):
         raise NotImplementedError("parse_trades is not implemented")
 
     def fix_position(self, raw, **kwargs):
         # add generic logic if necessary
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/basic_exchange_wrapper.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/basic_exchange_wrapper.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/config/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/config/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/config/backtesting_exchange_config.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/config/backtesting_exchange_config.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/config/exchange_config_data.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/config/exchange_config_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/ccxt/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/ccxt/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/ccxt/ccxt_adapter.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/ccxt/ccxt_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,15 @@
         return fixed
 
     def parse_public_recent_trades(self, fixed, **kwargs):
         # CCXT standard public_recent_trades parsing logic
         for recent_trade in fixed:
             recent_trade.pop(ecoc.INFO.value, None)
             recent_trade.pop(ecoc.DATETIME.value, None)
+            recent_trade.pop(ecoc.EXCHANGE_ID.value, None)
             recent_trade.pop(ecoc.ID.value, None)
             recent_trade.pop(ecoc.ORDER.value, None)
             recent_trade.pop(ecoc.FEE.value, None)
             recent_trade.pop(ecoc.TYPE.value, None)
             recent_trade.pop(ecoc.TAKER_OR_MAKER.value, None)
         return fixed
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/ccxt/ccxt_client_util.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/ccxt/ccxt_client_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/ccxt/ccxt_connector.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/ccxt/ccxt_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,20 +281,20 @@
             return self.all_currencies_price_ticker
         except ccxt.NotSupported:
             raise octobot_trading.errors.NotSupported
         except ccxt.BaseError as e:
             raise octobot_trading.errors.FailedRequest(f"Failed to get_all_currencies_price_ticker {e}")
 
     # ORDERS
-    async def get_order(self, order_id: str, symbol: str = None, **kwargs: dict) -> dict:
+    async def get_order(self, exchange_order_id: str, symbol: str = None, **kwargs: dict) -> dict:
         if self.client.has['fetchOrder']:
             try:
                 with self.error_describer():
                     return self.adapter.adapt_order(
-                        await self.client.fetch_order(order_id, symbol, params=kwargs),
+                        await self.client.fetch_order(exchange_order_id, symbol, params=kwargs),
                         symbol=symbol
                     )
             except ccxt.OrderNotFound:
                 # some exchanges are throwing this error when an order is cancelled (ex: coinbase pro)
                 pass
             except ccxt.NotSupported as e:
                 # some exchanges are throwing this error when an order is cancelled (ex: coinbase pro)
@@ -302,15 +302,15 @@
             except ccxt.ExchangeError as e:
                 # something went wrong and ccxt did not expect it
                 raise octobot_trading.errors.FailedRequest from e
         else:
             # When fetch_order is not supported, uses get_open_orders and extract order id
             open_orders = await self.get_open_orders(symbol=symbol)
             for order in open_orders:
-                if order.get(ecoc.ID.value, None) == order_id:
+                if order.get(ecoc.EXCHANGE_ID.value, None) == exchange_order_id:
                     return order
         return None  # OrderNotFound
 
     async def get_all_orders(self, symbol: str = None, since: int = None,
                              limit: int = None, **kwargs: dict) -> list:
         if self.client.has['fetchOrders']:
             with self.error_describer():
@@ -445,39 +445,41 @@
 
     async def create_market_trailing_stop_order(self, symbol, quantity, price=None, side=None, params=None) -> dict:
         raise NotImplementedError("create_market_trailing_stop_order is not implemented")
 
     async def create_limit_trailing_stop_order(self, symbol, quantity, price=None, side=None, params=None) -> dict:
         raise NotImplementedError("create_limit_trailing_stop_order is not implemented")
 
-    async def edit_order(self, order_id: str, order_type: enums.TraderOrderType, symbol: str,
+    async def edit_order(self, exchange_order_id: str, order_type: enums.TraderOrderType, symbol: str,
                          quantity: float, price: float, stop_price: float = None, side: str = None,
                          current_price: float = None, params: dict = None):
         ccxt_order_type = self.get_ccxt_order_type(order_type)
         price_to_use = price
         if ccxt_order_type == enums.TradeOrderType.MARKET.value:
             # can't set price in market orders
             price_to_use = None
         # do not use keyword arguments here as default ccxt edit order is passing *args (and not **kwargs)
         return self.adapter.adapt_order(
-            await self.client.edit_order(order_id, symbol, ccxt_order_type, side, quantity, price_to_use, params),
+            await self.client.edit_order(
+                exchange_order_id, symbol, ccxt_order_type, side, quantity, price_to_use, params
+            ),
             symbol=symbol
         )
 
     async def cancel_order(
-            self, order_id: str, symbol: str, order_type: enums.TraderOrderType, **kwargs: dict
+        self, exchange_order_id: str, symbol: str, order_type: enums.TraderOrderType, **kwargs: dict
     ) -> enums.OrderStatus:
         try:
             with self.error_describer():
-                await self.client.cancel_order(order_id, symbol=symbol, params=kwargs)
+                await self.client.cancel_order(exchange_order_id, symbol=symbol, params=kwargs)
                 # no exception, cancel worked
             try:
                 # make sure order is canceled
                 cancelled_order = await self.exchange_manager.exchange.get_order(
-                    order_id, symbol=symbol
+                    exchange_order_id, symbol=symbol
                 )
                 if cancelled_order is None or personal_data.parse_is_cancelled(cancelled_order):
                     return enums.OrderStatus.CANCELED
                 elif personal_data.parse_is_open(cancelled_order):
                     return enums.OrderStatus.PENDING_CANCEL
                 # cancel command worked but order is still existing and is not open or canceled. unhandled case
                 # log error and consider it canceling. order states will manage the
@@ -485,21 +487,21 @@
                                   f"Considered as {enums.OrderStatus.PENDING_CANCEL.value}")
                 return enums.OrderStatus.PENDING_CANCEL
             except ccxt.OrderNotFound:
                 # Order is not found: it has successfully been cancelled (some exchanges don't allow to
                 # get a cancelled order).
                 return enums.OrderStatus.CANCELED
         except ccxt.OrderNotFound as e:
-            self.logger.debug(f"Trying to cancel order with id {order_id} but order was not found")
+            self.logger.debug(f"Trying to cancel order with id {exchange_order_id} but order was not found")
             raise octobot_trading.errors.OrderCancelError from e
         except (ccxt.NotSupported, octobot_trading.errors.NotSupported) as e:
             raise octobot_trading.errors.NotSupported from e
         except Exception as e:
-            self.logger.exception(e, True, f"Unexpected error when cancelling order with id: "
-                                           f"{order_id} failed to cancel | {e} ({e.__class__.__name__})")
+            self.logger.exception(e, True, f"Unexpected error when cancelling order with exchange id: "
+                                           f"{exchange_order_id} failed to cancel | {e} ({e.__class__.__name__})")
             raise e
 
     async def get_positions(self, symbols=None, **kwargs: dict) -> list:
         try:
             return [
                 self.adapter.adapt_position(position)
                 for position in await self.client.fetch_positions(symbols=symbols, params=kwargs)
@@ -722,16 +724,16 @@
     def parse_timestamp(self, data_dict, timestamp_key, default_value=None, ms=False):
         parsed_timestamp = self.client.parse8601(self.client.safe_string(data_dict, timestamp_key))
         return (parsed_timestamp if ms else parsed_timestamp * 10 ** -3) if parsed_timestamp else default_value
 
     def parse_currency(self, currency):
         return self.client.safe_currency_code(currency)
 
-    def parse_order_id(self, order):
-        return order.get(ecoc.ID.value, None)
+    def parse_exhange_order_id(self, order):
+        return order.get(ecoc.EXCHANGE_ID.value, None)
 
     def parse_order_symbol(self, order):
         return order.get(ecoc.SYMBOL.value, None)
 
     def parse_side(self, side):
         return enums.TradeOrderSide.BUY if side == self.BUY_STR else enums.TradeOrderSide.SELL
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/ccxt/ccxt_websocket_connector.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/ccxt/ccxt_websocket_connector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/ccxt/constants.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/ccxt/constants.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/ccxt/enums.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/ccxt/enums.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/simulator/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/simulator/exchange_simulator_adapter.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/simulator/exchange_simulator_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/exchange_builder.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/exchange_builder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/exchange_channels.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/exchange_channels.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/exchange_factory.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/exchange_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/exchange_manager.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/exchange_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/exchange_websocket_factory.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/exchange_websocket_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/exchanges.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/exchanges.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/implementations/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/implementations/default_rest_exchange.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/implementations/default_rest_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/implementations/default_websocket_exchange.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/implementations/default_websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/implementations/exchange_simulator.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/implementations/exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/traders/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/traders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/traders/trader.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/traders/trader.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,15 @@
             quantity, price, stop_price and current_price
         Portfolio is updated within this call
         :return: True when an order field got updated
         """
         if not order.can_be_edited():
             raise errors.OrderEditError(f"Order can't be edited, order: {order}")
         changed = False
-        previous_order_id = order.order_id
+        previous_exchange_order_id = order.exchange_order_id
         try:
             async with order.lock:
                 # now that we got the lock, ensure we can edit the order
                 if not self.simulate and not order.is_self_managed() and order.state is not None:
                     # careful here: make sure we are not editing an order on exchange that is being updated
                     # somewhere else
                     async with order.state.refresh_operation():
@@ -179,15 +179,15 @@
                                          f"edited_stop_price: {str(edited_stop_price)} "
                                          f"edited_current_price: {str(edited_current_price)}"
                                          f"]")
                         order_params = self.exchange_manager.exchange.get_order_additional_params(order)
                         order_params.update(params or {})
                         # fill in every param as some exchange rely on re-creating the order altogether
                         edited_order = await self.exchange_manager.exchange.edit_order(
-                            order.order_id,
+                            order.exchange_order_id,
                             order.order_type,
                             order.symbol,
                             quantity=order.origin_quantity if edited_quantity is None else edited_quantity,
                             price=order.origin_price if edited_price is None else edited_price,
                             stop_price=edited_stop_price,
                             side=order.side,
                             current_price=edited_current_price,
@@ -218,17 +218,17 @@
                 # push order edit into orders channel as edit update
                 await self.exchange_manager.exchange_personal_data.handle_order_update_notification(
                     order, enums.OrderUpdateType.EDIT
                 )
                 self.logger.info(f"Edited order: {order}")
             return changed
         finally:
-            if previous_order_id != order.order_id:
+            if previous_exchange_order_id != order.exchange_order_id:
                 # order id changed: update orders_manager to keep consistency
-                self.exchange_manager.exchange_personal_data.orders_manager.replace_order(previous_order_id, order)
+                self.exchange_manager.exchange_personal_data.orders_manager.replace_order(order.order_id, order)
 
     async def _create_new_order(self, new_order, params: dict,
                                 wait_for_creation=True,
                                 creation_timeout=octobot_trading.constants.INDIVIDUAL_ORDER_SYNC_TIMEOUT) -> object:
         """
         Creates an exchange managed order, it might be a simulated or a real order.
         Portfolio will be updated by the created order state after order will be initialized
@@ -259,24 +259,23 @@
                 self, created_order, force_open_or_pending_creation=True
             )
             is_pending_creation = updated_order.status == enums.OrderStatus.PENDING_CREATION
 
             # rebind local elements to new order instance
             if new_order.order_group:
                 updated_order.add_to_order_group(new_order.order_group)
+            updated_order.order_id = new_order.order_id
             updated_order.tag = new_order.tag
             updated_order.chained_orders = new_order.chained_orders
             for chained_order in new_order.chained_orders:
                 chained_order.triggered_by = updated_order
-                chained_order.replace_associated_entry_id(new_order.order_id, updated_order.order_id)
             updated_order.triggered_by = new_order.triggered_by
             updated_order.has_been_bundled = new_order.has_been_bundled
             updated_order.exchange_creation_params = new_order.exchange_creation_params
             updated_order.is_waiting_for_chained_trigger = new_order.is_waiting_for_chained_trigger
-            updated_order.set_shared_signal_order_id(new_order.shared_signal_order_id)
             updated_order.associated_entry_ids = new_order.associated_entry_ids
             updated_order.update_with_triggering_order_fees = new_order.update_with_triggering_order_fees
 
             if is_pending_creation:
                 # register order as pending order, it will then be added to live orders in order manager once open
                 self.exchange_manager.exchange_personal_data.orders_manager.register_pending_creation_order(updated_order)
 
@@ -358,23 +357,23 @@
             return success
         # if real order: cancel on exchange
         if not self.simulate and not order.is_self_managed():
             try:
                 async with order.lock:
                     try:
                         order_status = await self.exchange_manager.exchange.cancel_order(
-                            order.order_id, order.symbol, order.order_type
+                            order.exchange_order_id, order.symbol, order.order_type
                         )
                     except errors.NotSupported:
                         raise
                     except (errors.OrderCancelError, Exception) as err:
                         # retry to cancel order
                         self.logger.debug(f"Failed to cancel order ({err} {err.__class__.__name__}), retrying")
                         order_status = await self.exchange_manager.exchange.cancel_order(
-                            order.order_id, order.symbol, order.order_type
+                            order.exchange_order_id, order.symbol, order.order_type
                         )
             except errors.OrderCancelError as err:
                 if await self._handle_order_cancel_error(order, err, wait_for_cancelling, cancelling_timeout):
                     return True
             except Exception as e:
                 self.logger.exception(e, True, f"Failed to cancel order {order}")
                 return False
@@ -440,27 +439,27 @@
             ) from err
 
     async def _wait_for_order_cancel(self, order, cancelling_timeout):
         self.logger.debug(f"Waiting for order cancelling, order: {order}")
         await order.state.wait_for_terminate(cancelling_timeout)
         self.logger.debug(f"Completed order cancelling, order: {order}")
 
-    async def cancel_order_with_id(self, order_id, emit_trading_signals=False,
+    async def cancel_order_with_id(self, exchange_order_id, emit_trading_signals=False,
                                    wait_for_cancelling=True,
                                    cancelling_timeout=octobot_trading.constants.INDIVIDUAL_ORDER_SYNC_TIMEOUT):
         """
         Gets order matching order_id from the OrderManager and calls self.cancel_order() on it
-        :param order_id: Id of the order to cancel
+        :param exchange_order_id: Exchange id of the order to cancel
         :param emit_trading_signals: when true, trading signals will be emitted
         :param wait_for_cancelling: when True, always make sure the order is completely cancelled before returning.
         :param cancelling_timeout: time before raising a timeout error when waiting for an order cancel
         :return: True if cancel is successful, False if order is not found or cancellation failed
         """
         try:
-            order = self.exchange_manager.exchange_personal_data.orders_manager.get_order(order_id)
+            order = self.exchange_manager.exchange_personal_data.orders_manager.get_order(exchange_order_id)
             async with signals.remote_signal_publisher(self.exchange_manager, order.symbol, emit_trading_signals):
                 return await signals.cancel_order(
                     self.exchange_manager,
                     emit_trading_signals and signals.should_emit_trading_signal(self.exchange_manager),
                     order,
                     wait_for_cancelling=wait_for_cancelling,
                     cancelling_timeout=cancelling_timeout,
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/traders/trader_simulator.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/traders/trader_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/types/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/types/rest_exchange.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/types/rest_exchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from octobot_trading.enums import ExchangeConstantsOrderColumns as ecoc
 import octobot_trading.exchanges.abstract_exchange as abstract_exchange
 import octobot_trading.exchange_data.contracts as contracts
 import octobot_trading.personal_data.orders as orders
 
 
 class RestExchange(abstract_exchange.AbstractExchange):
-    ORDER_NON_EMPTY_FIELDS = [ecoc.ID.value, ecoc.TIMESTAMP.value, ecoc.SYMBOL.value, ecoc.TYPE.value,
+    ORDER_NON_EMPTY_FIELDS = [ecoc.EXCHANGE_ID.value, ecoc.TIMESTAMP.value, ecoc.SYMBOL.value, ecoc.TYPE.value,
                               ecoc.SIDE.value, ecoc.PRICE.value, ecoc.AMOUNT.value, ecoc.STATUS.value]
     ORDER_REQUIRED_FIELDS = ORDER_NON_EMPTY_FIELDS + [ecoc.REMAINING.value]
     PRINT_DEBUG_LOGS = False
     REQUIRE_ORDER_FEES_FROM_TRADES = False  # set True when get_order is not giving fees on closed orders and fees
     # should be fetched using recent trades.
     REQUIRE_CLOSED_ORDERS_FROM_RECENT_TRADES = False  # set True when get_closed_orders is not supported
     ALLOW_TRADES_FROM_CLOSED_ORDERS = False  # set True when get_my_recent_trades should use get_closed_orders
@@ -139,40 +139,40 @@
                 order_type=order_type, symbol=symbol, quantity=quantity, price=price,
                 stop_price=stop_price, side=side, current_price=current_price,
                 reduce_only=reduce_only, params=params)
             self.logger.debug(f"Created order: {created_order}")
             return await self._verify_order(created_order, order_type, symbol, price, side)
         return None
 
-    async def edit_order(self, order_id: str, order_type: enums.TraderOrderType, symbol: str,
+    async def edit_order(self, exchange_order_id: str, order_type: enums.TraderOrderType, symbol: str,
                          quantity: decimal.Decimal, price: decimal.Decimal,
                          stop_price: decimal.Decimal = None, side: enums.TradeOrderSide = None,
                          current_price: decimal.Decimal = None,
                          params: dict = None):
         # Note: on most exchange, this implementation will just replace the order by cancelling the one
         # which id is given and create a new one
         async with self._order_operation(order_type, symbol, quantity, price, stop_price):
             float_quantity = float(quantity)
             float_price = float(price)
             float_stop_price = None if stop_price is None else float(stop_price)
             float_current_price = None if current_price is None else float(current_price)
             side = None if side is None else side.value
             params = {} if params is None else params
             params.update(self.exchange_manager.exchange_backend.get_orders_parameters(None))
-            edited_order = await self._edit_order(order_id, order_type, symbol, quantity=float_quantity,
+            edited_order = await self._edit_order(exchange_order_id, order_type, symbol, quantity=float_quantity,
                                                   price=float_price, stop_price=float_stop_price, side=side,
                                                   current_price=float_current_price, params=params)
             order = await self._verify_order(edited_order, order_type, symbol, price, side)
             return order
         return None
 
-    async def _edit_order(self, order_id: str, order_type: enums.TraderOrderType, symbol: str,
+    async def _edit_order(self, exchange_order_id: str, order_type: enums.TraderOrderType, symbol: str,
                           quantity: float, price: float, stop_price: float = None, side: str = None,
                           current_price: float = None, params: dict = None):
-        return await self.connector.edit_order(order_id, order_type, symbol,
+        return await self.connector.edit_order(exchange_order_id, order_type, symbol,
                                                quantity, price, stop_price, side,
                                                current_price, params)
 
     @contextlib.asynccontextmanager
     async def _order_operation(self, order_type, symbol, quantity, price, stop_price):
         try:
             yield
@@ -192,22 +192,22 @@
             self.log_order_creation_error(e, order_type, symbol, quantity, price, stop_price)
             print(traceback.format_exc(), file=sys.stderr)
             self.logger.exception(e, False, f"Unexpected error during order operation: {e}")
 
     async def _verify_order(self, created_order, order_type, symbol, price, side, get_order_params=None):
         # some exchanges are not returning the full order details on creation: fetch it if necessary
         if created_order and not self._ensure_order_details_completeness(created_order):
-            if ecoc.ID.value in created_order:
-                order_id = created_order[ecoc.ID.value]
-                if order_id is None:
-                    self.logger.error(f"No order id on created order: {created_order}")
+            if ecoc.EXCHANGE_ID.value in created_order:
+                order_exchange_id = created_order[ecoc.EXCHANGE_ID.value]
+                if order_exchange_id is None:
+                    self.logger.error(f"No order exchange id on created order: {created_order}")
                     return None
                 params = get_order_params or {}
                 fetched_order = await self.get_order(
-                    created_order[ecoc.ID.value], symbol=symbol, **params
+                    created_order[ecoc.EXCHANGE_ID.value], symbol=symbol, **params
                 )
                 if fetched_order is None:
                     created_order[ecoc.STATUS.value] = enums.OrderStatus.PENDING_CREATION.value
                     # Order is created but not live on exchange. Consider it as pending.
                     # It will be updated later on via order updater
                     created_order[ecoc.SYMBOL.value] = symbol
                     created_order[ecoc.TYPE.value] = orders.get_trade_order_type(order_type).value
@@ -442,35 +442,35 @@
 
     async def get_price_ticker(self, symbol: str, **kwargs: dict) -> typing.Optional[dict]:
         return await self.connector.get_price_ticker(symbol=symbol, **kwargs)
 
     async def get_all_currencies_price_ticker(self, **kwargs: dict) -> typing.Optional[list]:
         return await self.connector.get_all_currencies_price_ticker(**kwargs)
 
-    async def get_order(self, order_id: str, symbol: str = None, **kwargs: dict) -> dict:
+    async def get_order(self, exchange_order_id: str, symbol: str = None, **kwargs: dict) -> dict:
         return await self._ensure_order_completeness(
-            await self.connector.get_order(order_id, symbol=symbol, **kwargs),
+            await self.connector.get_order(exchange_order_id, symbol=symbol, **kwargs),
             symbol, **kwargs
         )
 
-    async def get_order_from_open_and_closed_orders(self, order_id: str, symbol: str = None, **kwargs: dict) -> dict:
+    async def get_order_from_open_and_closed_orders(self, exchange_order_id: str, symbol: str = None, **kwargs: dict) -> dict:
         for order in await self.get_open_orders(symbol, **kwargs):
-            if order[enums.ExchangeConstantsOrderColumns.ID.value] == order_id:
+            if order[enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value] == exchange_order_id:
                 return order
         for order in await self.get_closed_orders(symbol, **kwargs):
-            if order[enums.ExchangeConstantsOrderColumns.ID.value] == order_id:
+            if order[enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value] == exchange_order_id:
                 return order
         return None  # OrderNotFound
 
-    async def get_order_from_trades(self, symbol, order_id, order_to_update=None):
+    async def get_order_from_trades(self, symbol, exchange_order_id, order_to_update=None):
         order_to_update = order_to_update or {}
         trades = await self.get_my_recent_trades(symbol)
         # usually the right trade is within the last ones
         for trade in trades[::-1]:
-            if trade[ecoc.ORDER.value] == order_id:
+            if trade[ecoc.ORDER.value] == exchange_order_id:
                 return exchanges_util.update_raw_order_from_raw_trade(order_to_update, trade)
         return None  #OrderNotFound
 
     async def get_all_orders(self, symbol: str = None, since: int = None, limit: int = None, **kwargs: dict) -> list:
         return await self._ensure_orders_completeness(
             await self.connector.get_all_orders(symbol=symbol, since=since, limit=limit, **kwargs),
             symbol, since=since, limit=limit, **kwargs
@@ -501,55 +501,57 @@
         trades = await self.get_my_recent_trades(symbol, since=since, limit=limit, **kwargs)
         return [
             exchanges_util.update_raw_order_from_raw_trade({}, trade)
             for trade in trades
         ]
 
     async def _ensure_orders_completeness(
-        self, raw_orders, symbol, since=None, limit=None, trades_by_order_id=None, **kwargs
+        self, raw_orders, symbol, since=None, limit=None, trades_by_exchange_order_id=None, **kwargs
     ):
         if not self.REQUIRE_ORDER_FEES_FROM_TRADES \
                 or not any(exchanges_util.is_missing_trading_fees(order) for order in raw_orders):
             return raw_orders
-        trades_by_order_id = trades_by_order_id or await self._get_trades_by_order_id(
+        trades_by_exchange_order_id = trades_by_exchange_order_id or await self._get_trades_by_exchange_order_id(
             symbol=symbol, since=since, limit=limit, **kwargs
         )
         return [
-            await self._ensure_order_completeness(order, symbol, trades_by_order_id=trades_by_order_id, **kwargs)
+            await self._ensure_order_completeness(
+                order, symbol, trades_by_exchange_order_id=trades_by_exchange_order_id, **kwargs
+            )
             for order in raw_orders
         ]
 
     async def _ensure_order_completeness(
-        self, raw_order, symbol, since=None, limit=None, trades_by_order_id=None, **kwargs
+        self, raw_order, symbol, since=None, limit=None, trades_by_exchange_order_id=None, **kwargs
     ):
         if not self.REQUIRE_ORDER_FEES_FROM_TRADES or not exchanges_util.is_missing_trading_fees(raw_order):
             return raw_order
-        trades_by_order_id = trades_by_order_id or await self._get_trades_by_order_id(
+        trades_by_exchange_order_id = trades_by_exchange_order_id or await self._get_trades_by_exchange_order_id(
             symbol=symbol, since=since, limit=limit, **kwargs
         )
-        exchanges_util.apply_trades_fees(raw_order, trades_by_order_id)
+        exchanges_util.apply_trades_fees(raw_order, trades_by_exchange_order_id)
         return raw_order
 
-    async def _get_trades_by_order_id(self, symbol=None, since=None, limit=None, **kwargs):
-        trades_by_order_id = {}
+    async def _get_trades_by_exchange_order_id(self, symbol=None, since=None, limit=None, **kwargs):
+        trades_by_exchange_order_id = {}
         for trade in await self.get_my_recent_trades(symbol=symbol, since=since, limit=limit, **kwargs):
-            order_id = trade[enums.ExchangeConstantsOrderColumns.ORDER.value]
-            if order_id in trades_by_order_id:
-                trades_by_order_id[order_id].append(trade)
+            exchange_order_id = trade[enums.ExchangeConstantsOrderColumns.ORDER.value]
+            if exchange_order_id in trades_by_exchange_order_id:
+                trades_by_exchange_order_id[exchange_order_id].append(trade)
             else:
-                trades_by_order_id[order_id] = [trade]
-        return trades_by_order_id
+                trades_by_exchange_order_id[exchange_order_id] = [trade]
+        return trades_by_exchange_order_id
 
     async def get_my_recent_trades(self, symbol: str = None, since: int = None, limit: int = None, **kwargs: dict) -> list:
         return await self.connector.get_my_recent_trades(symbol=symbol, since=since, limit=limit, **kwargs)
 
     async def cancel_order(
-            self, order_id: str, symbol: str, order_type: enums.TraderOrderType, **kwargs: dict
+            self, exchange_order_id: str, symbol: str, order_type: enums.TraderOrderType, **kwargs: dict
     ) -> enums.OrderStatus:
-        return await self.connector.cancel_order(order_id, symbol, order_type, **kwargs)
+        return await self.connector.cancel_order(exchange_order_id, symbol, order_type, **kwargs)
 
     def get_trade_fee(self, symbol, order_type, quantity, price, taker_or_maker):
         return self.connector.get_trade_fee(symbol, order_type, quantity, price, taker_or_maker)
 
     def get_fees(self, symbol):
         return self.connector.get_fees(symbol)
 
@@ -832,16 +834,16 @@
     """
     Parsers todo remove ?
     """
 
     def parse_order_book_ticker(self, order_book_ticker):
         return self.connector.parse_order_book_ticker(order_book_ticker)
 
-    def parse_order_id(self, order):
-        return self.connector.parse_order_id(order)
+    def parse_exhange_order_id(self, order):
+        return self.connector.parse_exhange_order_id(order)
 
     def parse_order_symbol(self, order):
         return self.connector.parse_order_symbol(order)
 
     def parse_funding(self, funding_dict, from_ticker=False) -> dict:
         """
         :param from_ticker: when True, the funding dict is extracted from ticker data
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/types/websocket_exchange.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/types/websocket_exchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import asyncio
+import sys
 import concurrent.futures as futures
 
 import octobot_commons.thread_util as thread_util
 import octobot_trading.enums
 import octobot_trading.exchanges.abstract_websocket_exchange as abstract_websocket
 
 
@@ -130,15 +131,16 @@
         ])
 
     async def start_sockets(self):
         if any(self.handled_feeds.values() and self.websocket_connectors):
             try:
                 self.websocket_connectors_executors = futures.ThreadPoolExecutor(
                     max_workers=len(self.websocket_connectors),
-                    thread_name_prefix=f"{self.get_name()}-{self.exchange_name}-pool-executor"
+                    thread_name_prefix=f"{self.get_name()}-{self.exchange_name}-pool-executor",
+
                 )
 
                 self.websocket_connectors_tasks = [
                     asyncio.get_event_loop().run_in_executor(self.websocket_connectors_executors, websocket.start)
                     for websocket in self.websocket_connectors
                 ]
 
@@ -197,15 +199,18 @@
         try:
             for websocket in self.websocket_connectors:
                 await websocket.close()
         except Exception as e:
             self.logger.error(f"Error when closing sockets : {e}")
         for websocket_task in self.websocket_connectors_tasks:
             websocket_task.cancel()
-        thread_util.stop_thread_pool_executor_non_gracefully(self.websocket_connectors_executors)
+        if sys.version_info.minor >= 9:
+            self.websocket_connectors_executors.shutdown(True)
+        else:
+            thread_util.stop_thread_pool_executor_non_gracefully(self.websocket_connectors_executors)
         self.websocket_connectors_executors = None
 
     def add_pairs(self, pairs, watching_only=False):
         for websocket in self.websocket_connectors:
             websocket.add_pairs(pairs, watching_only=watching_only)
 
     def clear(self):
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/util/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/util/exchange_market_status_fixer.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/util/exchange_market_status_fixer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/util/exchange_util.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/util/exchange_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -245,15 +245,15 @@
         return [enums.ExchangeTypes.SPOT]
     return exchange_class.get_supported_exchange_types()
 
 
 def update_raw_order_from_raw_trade(order_to_update, raw_trade):
     order_to_update[enums.ExchangeConstantsOrderColumns.INFO.value] = raw_trade[
         enums.ExchangeConstantsOrderColumns.INFO.value]
-    order_to_update[enums.ExchangeConstantsOrderColumns.ID.value] = raw_trade[
+    order_to_update[enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value] = raw_trade[
         enums.ExchangeConstantsOrderColumns.ORDER.value]
     order_to_update[enums.ExchangeConstantsOrderColumns.SYMBOL.value] = raw_trade[
         enums.ExchangeConstantsOrderColumns.SYMBOL.value]
     order_to_update[enums.ExchangeConstantsOrderColumns.TYPE.value] = raw_trade[
         enums.ExchangeConstantsOrderColumns.TYPE.value]
     order_to_update[enums.ExchangeConstantsOrderColumns.AMOUNT.value] = raw_trade[
         enums.ExchangeConstantsOrderColumns.AMOUNT.value]
@@ -295,19 +295,19 @@
                 ] is None
             )
         )
     except KeyError:
         return True
 
 
-def apply_trades_fees(raw_order, raw_trades_by_order_id):
-    order_id = raw_order[enums.ExchangeConstantsOrderColumns.ID.value]
-    if order_id in raw_trades_by_order_id and raw_trades_by_order_id[order_id]:
-        order_fee = raw_trades_by_order_id[order_id][0][enums.ExchangeConstantsOrderColumns.FEE.value]
+def apply_trades_fees(raw_order, raw_trades_by_exchange_order_id):
+    exchange_order_id = raw_order[enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value]
+    if exchange_order_id in raw_trades_by_exchange_order_id and raw_trades_by_exchange_order_id[exchange_order_id]:
+        order_fee = raw_trades_by_exchange_order_id[exchange_order_id][0][enums.ExchangeConstantsOrderColumns.FEE.value]
         # add each order's trades fee
-        for trade in raw_trades_by_order_id[order_id][1:]:
+        for trade in raw_trades_by_exchange_order_id[exchange_order_id][1:]:
             order_fee[enums.FeePropertyColumns.COST.value] += \
                 trade[enums.ExchangeConstantsOrderColumns.FEE.value][enums.FeePropertyColumns.COST.value]
             order_fee[enums.FeePropertyColumns.EXCHANGE_ORIGINAL_COST.value] += \
                 trade[enums.ExchangeConstantsOrderColumns.FEE.value][
                     enums.FeePropertyColumns.EXCHANGE_ORIGINAL_COST.value]
         raw_order[enums.ExchangeConstantsOrderColumns.FEE.value] = order_fee
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/exchanges/util/websockets_util.py` & `OctoBot-Trading-2.4.3/octobot_trading/exchanges/util/websockets_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/abstract_trading_mode.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/abstract_trading_mode.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/channel/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/channel/abstract_mode_consumer.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/channel/abstract_mode_consumer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/channel/abstract_mode_producer.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/channel/abstract_mode_producer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/channel/mode.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/channel/mode.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/mode_config.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/mode_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,26 +52,31 @@
                                                                    f"the activated trading mode: {e}")
 
     raise errors.ConfigTradingError(f"Please ensure your tentacles configuration file is valid and "
                                     f"at least one trading mode is activated")
 
 
 def should_emit_trading_signals_user_input(trading_mode, inputs: dict):
-    if trading_mode.UI.user_input(
+    trading_mode.UI.user_input(
         common_constants.CONFIG_EMIT_TRADING_SIGNALS, common_enums.UserInputTypes.BOOLEAN, False, inputs,
         title="Emit trading signals on OctoBot cloud for people to follow.",
         order=commons_configuration.UserInput.MAX_ORDER - 2
-    ):
-        trading_mode.UI.user_input(
-            common_constants.CONFIG_TRADING_SIGNALS_STRATEGY, common_enums.UserInputTypes.TEXT, trading_mode.get_name(),
-            inputs,
-            title="Name of the strategy to send signals on.",
-            order=commons_configuration.UserInput.MAX_ORDER - 1,
-            other_schema_values={"minLength": 0},
-        )
+    )
+    trading_mode.UI.user_input(
+        common_constants.CONFIG_TRADING_SIGNALS_STRATEGY, common_enums.UserInputTypes.TEXT, trading_mode.get_name(),
+        inputs,
+        title="Name of the strategy to send signals on.",
+        order=commons_configuration.UserInput.MAX_ORDER - 1,
+        other_schema_values={"minLength": 0},
+        editor_options={
+            common_enums.UserInputOtherSchemaValuesTypes.DEPENDENCIES.value: {
+                common_constants.CONFIG_EMIT_TRADING_SIGNALS: True
+            }
+        }
+    )
 
 
 def is_trading_signal_emitter(trading_mode) -> bool:
     """
     :return: True if the mode should be emitting trading signals according to configuration
     """
     try:
@@ -93,22 +98,26 @@
 def user_select_order_amount(trading_mode, inputs: dict, include_buy=True, include_sell=True,
                              buy_dependencies=None, sell_dependencies=None):
     if include_buy:
         trading_mode.UI.user_input(
             constants.CONFIG_BUY_ORDER_AMOUNT, common_enums.UserInputTypes.TEXT, "", inputs,
             title=_get_order_amount_title("buy"),
             other_schema_values={"minLength": 0},
-            editor_options={"dependencies": buy_dependencies} if buy_dependencies else None,
+            editor_options={
+                common_enums.UserInputOtherSchemaValuesTypes.DEPENDENCIES.value: buy_dependencies
+            } if buy_dependencies else None,
         )
     if include_sell:
         trading_mode.UI.user_input(
             constants.CONFIG_SELL_ORDER_AMOUNT, common_enums.UserInputTypes.TEXT, "", inputs,
             title=_get_order_amount_title("sell"),
             other_schema_values={"minLength": 0},
-            editor_options={"dependencies": sell_dependencies} if sell_dependencies else None,
+            editor_options={
+                common_enums.UserInputOtherSchemaValuesTypes.DEPENDENCIES.value: sell_dependencies
+            } if sell_dependencies else None,
         )
 
 
 def get_user_selected_order_amount(trading_mode, side) -> str:
     try:
         if side is enums.TradeOrderSide.SELL:
             return trading_mode.trading_config[constants.CONFIG_SELL_ORDER_AMOUNT]
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/modes_factory.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/modes_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/modes_util.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/modes_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/basic_keywords/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/basic_keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/basic_keywords/account_balance.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/basic_keywords/account_balance.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/basic_keywords/amount.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/basic_keywords/amount.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/basic_keywords/configuration.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/basic_keywords/configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/basic_keywords/run_persistence.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/basic_keywords/run_persistence.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/basic_keywords/trading_signals.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/basic_keywords/trading_signals.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/basic_keywords/user_inputs.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/basic_keywords/user_inputs.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/context_management.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/context_management.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/dsl/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/dsl/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/dsl/quantity.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/dsl/quantity.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/script_keywords/dsl/values.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/script_keywords/dsl/values.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/scripted_trading_mode/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/scripted_trading_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/modes/scripted_trading_mode/abstract_scripted_trading_mode.py` & `OctoBot-Trading-2.4.3/octobot_trading/modes/scripted_trading_mode/abstract_scripted_trading_mode.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/octobot_channel_consumer.py` & `OctoBot-Trading-2.4.3/octobot_trading/octobot_channel_consumer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/exchange_personal_data.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/exchange_personal_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import octobot_trading.exchange_channel as exchange_channel
 import octobot_trading.constants as constants
 import octobot_trading.errors as errors
 import octobot_trading.enums as enums
 import octobot_trading.personal_data.portfolios.portfolio_manager as portfolio_manager
 import octobot_trading.personal_data.positions.positions_manager as positions_manager
 import octobot_trading.personal_data.orders.orders_manager as orders_manager
+import octobot_trading.personal_data.orders.order as order_import
 import octobot_trading.personal_data.orders.orders_storage_operations as orders_storage_operations
 import octobot_trading.personal_data.trades.trades_manager as trades_manager
 import octobot_trading.personal_data.transactions.transactions_manager as transactions_manager
 import octobot_trading.personal_data.transactions.transaction_factory as transaction_factory
 import octobot_trading.util as util
 
 
@@ -164,60 +165,61 @@
                     .send(profitability=portfolio_profitability.profitability,
                           profitability_percent=portfolio_profitability.profitability_percent,
                           market_profitability_percent=portfolio_profitability.market_profitability_percent,
                           initial_portfolio_current_profitability=portfolio_profitability.initial_portfolio_current_profitability)
         except Exception as e:
             self.logger.exception(e, True, f"Failed to update portfolio profitability : {e}")
 
-    async def handle_order_update_from_raw(self, order_id, raw_order,
+    async def handle_order_update_from_raw(self, exchange_order_id, raw_order,
                                            is_new_order: bool = False,
                                            should_notify: bool = True,
-                                           is_from_exchange=True) -> bool:
+                                           is_from_exchange=True) -> (bool, order_import.Order):
         # Orders can sometimes be out of sync between different exchange endpoints (ex: binance order API vs
         # open_orders API which is slower).
         # Always check if this order has not already been closed previously (most likely during the last
         # seconds/minutes)
-        if self._is_out_of_sync_order(order_id):
-            self.logger.debug(f"Ignored update for order with {order_id}: this order has already been closed "
-                              f"(received raw order: {raw_order})")
+        if self._is_out_of_sync_order(exchange_order_id):
+            self.logger.debug(f"Ignored update for order with exchange id: {exchange_order_id}: this order "
+                              f"has already been closed (received raw order: {raw_order})")
         else:
             try:
-                changed: bool = await self.orders_manager.upsert_order_from_raw(order_id, raw_order, is_from_exchange)
+                changed, order = await self.orders_manager.upsert_order_from_raw(
+                    exchange_order_id, raw_order, is_from_exchange
+                )
                 if changed:
-                    updated_order = self.orders_manager.get_order(order_id)
-                    await self.on_order_refresh_success(updated_order, should_notify, is_new_order)
-                return changed
+                    await self.on_order_refresh_success(order, should_notify, is_new_order)
+                return changed, order
             except errors.PortfolioNegativeValueError as e:
                 if is_new_order:
                     self.logger.debug(f"Impossible to count new order in portfolio: a synch is necessary "
                                       f"(order: {raw_order}).")
                     # forward to caller: this is a new order: portfolio might not be synchronized
                     raise
                 self.logger.exception(e, True, f"Failed to update order : {e}")
             except KeyError as ke:
                 self.logger.debug(f"Failed to update order : Order was not found ({ke})")
             except Exception as e:
                 self.logger.exception(e, True, f"Failed to update order : {e}")
-        return False
+        return False, None
 
-    async def update_order_from_stored_data(self, order_id, pending_groups):
-        order = self.orders_manager.get_order(order_id)
+    async def update_order_from_stored_data(self, exchange_order_id, pending_groups):
+        order = self.orders_manager.get_order(None, exchange_order_id=exchange_order_id)
         await orders_storage_operations.apply_order_storage_details_if_any(order, self.exchange_manager, pending_groups)
 
     async def on_order_refresh_success(self, order, should_notify, is_new_order):
         if order.state is not None:
             asyncio.create_task(order.state.on_refresh_successful())
 
         if should_notify:
             update_type = enums.OrderUpdateType.NEW if is_new_order else enums.OrderUpdateType.STATE_CHANGE
             await self.handle_order_update_notification(order, update_type)
         return order.state is not None
 
-    def _is_out_of_sync_order(self, order_id) -> bool:
-        return self.trades_manager.has_closing_trade_with_order_id(order_id)
+    def _is_out_of_sync_order(self, exchange_order_id) -> bool:
+        return self.trades_manager.has_closing_trade_with_exchange_order_id(exchange_order_id)
 
     async def handle_order_instance_update(self, order, is_new_order: bool = False, should_notify: bool = True):
         try:
             changed: bool = await self.orders_manager.upsert_order_instance(order)
 
             if changed:
                 await self.on_order_refresh_success(order, should_notify, is_new_order)
@@ -244,23 +246,23 @@
                 is_from_bot=order.is_from_this_octobot,
                 update_type=update_type,
                 is_closed=order.is_closed()
             )
         except ValueError as e:
             self.logger.error(f"Failed to send order update notification : {e}")
 
-    async def handle_closed_order_update(self, order_id, raw_order) -> bool:
+    async def handle_closed_order_update(self, exchange_order_id, raw_order) -> bool:
         """
         Handle closed order creation or update
-        :param order_id: the closed order id
+        :param exchange_order_id: the closed order id on exchange
         :param raw_order: the closed order dict
         :return: True if the closed order has been created or updated
         """
         try:
-            found_order = await self.orders_manager.upsert_order_close_from_raw(order_id, raw_order)
+            found_order = await self.orders_manager.upsert_order_close_from_raw(exchange_order_id, raw_order)
             if found_order is None:
                 return False
             await self.on_order_refresh_success(found_order, False, False)
             return True
         except Exception as e:
             self.logger.exception(e, True, f"Failed to update order : {e}")
             return False
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/channel/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/channel/orders.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/channel/orders.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,36 +36,36 @@
             pending_groups = {}  # Used when restoring orders from order storage:
             # a dict of order groups for which to check if associated self-managed orders are to be created
             for order in orders:
                 symbol = self.channel.exchange_manager.get_exchange_symbol(
                     self.channel.exchange_manager.exchange.parse_order_symbol(order)
                 )
                 symbols.add(symbol)
-                order_id: str = self.channel.exchange_manager.exchange.parse_order_id(order)
+                exchange_order_id: str = self.channel.exchange_manager.exchange.parse_exhange_order_id(order)
 
                 # if this order was not managed by order_manager before
                 is_new_order = not self.channel.exchange_manager.exchange_personal_data.orders_manager. \
-                    has_order(order_id)
+                    has_order(None, exchange_order_id=exchange_order_id)
                 has_new_order |= is_new_order
 
                 # update this order
                 if are_closed:
-                    await self._handle_close_order_update(order_id, order)
+                    await self._handle_close_order_update(exchange_order_id, order)
                 else:
                     try:
                         # will add a group to pending_groups if a group is restored from orders storage
                         await self._handle_open_order_update(
-                            symbol, order, order_id, is_from_bot, is_new_order, pending_groups
+                            symbol, order, exchange_order_id, is_from_bot, is_new_order, pending_groups
                         )
                     except errors.PortfolioNegativeValueError:
                         # Special case for new orders: their order init does not finish properly when this happens
                         if is_new_order and self.channel.exchange_manager.exchange_personal_data.orders_manager. \
-                           has_order(order_id):
+                           has_order(None, exchange_order_id=exchange_order_id):
                             new_order = self.channel.exchange_manager.exchange_personal_data.orders_manager.get_order(
-                                order_id
+                                None, exchange_order_id=exchange_order_id
                             )
                             # Order init might have failed due to a portfolio update on the exchange side
                             # (added funds, etc).
                             waiting_complete_init_orders.append(new_order)
                         else:
                             # order was not even added to orders_manager: another issue happened, raise
                             raise
@@ -79,41 +79,45 @@
                 )
 
         except asyncio.CancelledError:
             self.logger.info("Update tasks cancelled.")
         except Exception as e:
             self.logger.exception(e, True, f"Exception when triggering update: {e}")
 
-    async def _handle_open_order_update(self, symbol, order, order_id, is_from_bot, is_new_order, pending_groups):
+    async def _handle_open_order_update(
+        self, symbol, order_dict, exchange_order_id, is_from_bot, is_new_order, pending_groups
+    ):
         """
         Create or update an open Order from exchange data
         :param symbol: the order symbol
-        :param order: the order dict
-        :param order_id: the order id
+        :param order_dict: the order dict
+        :param exchange_order_id: the order id on exchange
         :param is_from_bot: If the order was created by OctoBot
         :param is_new_order: True if this open order has been created
         :param pending_groups: dict of groups to be created
         """
-        if (await self.channel.exchange_manager.exchange_personal_data.handle_order_update_from_raw(
-                order_id, order, is_new_order=is_new_order, should_notify=False)):
+        changed, order = await self.channel.exchange_manager.exchange_personal_data.handle_order_update_from_raw(
+            exchange_order_id, order_dict, is_new_order=is_new_order, should_notify=False
+        )
+        if changed:
             if is_new_order and \
                     not self.channel.exchange_manager.exchange_personal_data.orders_manager.\
                     are_exchange_orders_initialized:
                 try:
                     # when fetching initial orders, complete them with storage data when possible
                     await self.channel.exchange_manager.exchange_personal_data.update_order_from_stored_data(
-                        order_id,
+                        order.exchange_order_id,
                         pending_groups,
                     )
                 except Exception as err:
                     self.logger.exception(err, True, f"Error when completing order with stored data: {err}")
             await self.send(
                 self.channel.exchange_manager.exchange.get_pair_cryptocurrency(symbol),
                 symbol,
-                order,
+                order.to_dict(),
                 is_from_bot=is_from_bot,
                 update_type=enums.OrderUpdateType.NEW if is_new_order else enums.OrderUpdateType.STATE_CHANGE,
                 is_closed=False
             )
 
     async def _complete_open_order_init(self, orders, is_from_bot):
         """
@@ -127,21 +131,23 @@
                 order.symbol,
                 order.to_dict(),
                 is_from_bot=is_from_bot,
                 update_type=enums.OrderUpdateType.NEW,
                 is_closed=False
             )
 
-    async def _handle_close_order_update(self, order_id, order):
+    async def _handle_close_order_update(self, exchange_order_id, raw_order):
         """
         Create or update a close Order from exchange data
-        :param order: the order dict
-        :param order_id: the order id
+        :param exchange_order_id: the order id
+        :param raw_order: the order dict
         """
-        await self.channel.exchange_manager.exchange_personal_data.handle_closed_order_update(order_id, order)
+        await self.channel.exchange_manager.exchange_personal_data.handle_closed_order_update(
+            exchange_order_id, raw_order
+        )
 
     async def handle_post_open_orders_update(
             self, symbols, orders, waiting_complete_init_orders, has_new_order, is_from_bot
     ):
         """
         Perform post open Order update actions :
         - 1. Check if some previously known open order has not been found during update
@@ -204,24 +210,25 @@
         """
         Check if there is no missing open orders in order_manager compared to exchange open orders
         :param symbol: the order symbol
         :param orders: open orders from exchange
         """
         missing_order_ids = list(
             set(
-                order.order_id for order in
+                order.exchange_order_id for order in
                 self.channel.exchange_manager.exchange_personal_data.orders_manager.get_open_orders(
                     symbol
                 ) + self.channel.exchange_manager.exchange_personal_data.orders_manager.get_pending_cancel_orders(
                     symbol
                 )
                 if not (order.is_cleared() or order.is_self_managed())) -
             set(
-                self.channel.exchange_manager.exchange.parse_order_id(order)
-                for order in orders)
+                self.channel.exchange_manager.exchange.parse_exhange_order_id(order)
+                for order in orders
+            )
         )
         if missing_order_ids:
             self.logger.debug(f"{len(missing_order_ids)} open orders are missing on exchange, "
                               f"synchronizing with exchange...")
             synchronize_tasks = []
             for missing_order_id in missing_order_ids:
                 try:
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/channel/orders_updater.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/channel/orders_updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,21 +183,21 @@
         Update Order from exchange
         :param order: the order to update
         :param should_notify: if Orders channel consumers should be notified
         :return: True if the order was updated
         """
         exchange_name = order.exchange_manager.exchange_name if order.exchange_manager else "cleared order's exchange"
         self.logger.debug(f"Requested update for {order} on {exchange_name}")
-        raw_order = await self.channel.exchange_manager.exchange.get_order(order.order_id, order.symbol)
+        raw_order = await self.channel.exchange_manager.exchange.get_order(order.exchange_order_id, order.symbol)
 
         if raw_order is not None:
             self.logger.debug(f"Received update for {order} on {exchange_name}: {raw_order}")
 
             await self.channel.exchange_manager.exchange_personal_data.handle_order_update_from_raw(
-                order.order_id, raw_order, should_notify=should_notify
+                order.exchange_order_id, raw_order, should_notify=should_notify
             )
         else:
             self.logger.debug(f"Can't received update for {order} on {exchange_name}: received order is None")
 
     async def stop(self) -> None:
         """
         Stop producer by stopping its jobs
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/channel/orders_updater_simulator.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/channel/orders_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/decimal_order_adapter.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/decimal_order_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/groups/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/groups/group_util.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/groups/group_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/order.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/order.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import asyncio
 import typing
 import contextlib
 import decimal
-import uuid
 
 import octobot_commons.logging as logging
 
 import octobot_trading.constants as constants
 import octobot_trading.enums as enums
 import octobot_trading.errors as errors
 import octobot_trading.personal_data.orders.states as orders_states
@@ -44,16 +43,16 @@
         self.exchange_manager = trader.exchange_manager
         self.lock = asyncio.Lock()
         self.is_synchronized_with_exchange = False
         self.is_from_this_octobot = True
         self.simulated = trader.simulate
 
         self.logger_name = None
-        self.order_id = trader.parse_order_id(None)
-        self.shared_signal_order_id = str(uuid.uuid4())
+        self.order_id = order_util.generate_order_id()        # used id; kept through instances and trading signals
+        self.exchange_order_id = trader.parse_order_id(None)  # given by the exchange, local to the user account
         self.status = enums.OrderStatus.OPEN
         self.symbol = None
         self.currency = None
         self.market = None
         self.quantity_currency = None
         self.taker_or_maker = None
         self.timestamp = 0
@@ -121,32 +120,35 @@
 
     @classmethod
     def get_name(cls):
         return cls.__name__
 
     def get_logger_name(self):
         if self.logger_name is None:
-            self.logger_name = f"{self.get_name()} | {self.order_id}"
+            self.logger_name = f"{self.get_name()} | {self.order_id} [exchange id: {self.exchange_order_id}]"
         return self.logger_name
 
-    def update(self, symbol, order_id="", status=enums.OrderStatus.OPEN,
+    def update(self, symbol, order_id="", exchange_order_id=None, status=enums.OrderStatus.OPEN,
                current_price=constants.ZERO, quantity=constants.ZERO, price=constants.ZERO, stop_price=constants.ZERO,
                quantity_filled=constants.ZERO, filled_price=constants.ZERO, average_price=constants.ZERO,
                fee=None, total_cost=constants.ZERO, timestamp=None,
                order_type=None, reduce_only=None, close_position=None, position_side=None, fees_currency_side=None,
                group=None, tag=None, quantity_currency=None, exchange_creation_params=None,
                associated_entry_id=None) -> bool:
         changed: bool = False
         should_update_total_cost = False
 
         price = current_price if self.use_current_price_as_origin_price() else price
 
         if order_id and self.order_id != order_id:
             self.order_id = order_id
 
+        if exchange_order_id and self.exchange_order_id != exchange_order_id:
+            self.exchange_order_id = exchange_order_id
+
         if symbol and self.symbol != symbol:
             self.currency, self.market = self.exchange_manager.get_exchange_quote_and_base(symbol)
             self.symbol = symbol
 
         if quantity_currency is None:
             if self.quantity_currency is None and self.symbol is not None:
                 self.quantity_currency = order_util.get_order_quantity_currency(self.exchange_manager, self.symbol)
@@ -285,20 +287,14 @@
         """
         Called when origin price just changed.
         Override if necessary
         :param previous_price: the previous origin_price
         :param price_time: time starting from when the price should be considered
         """
 
-    def set_shared_signal_order_id(self, shared_signal_order_id):
-        """
-        Updates the local shared_signal_order_id. Should only be called on orders originated from trading signals
-        """
-        self.shared_signal_order_id = shared_signal_order_id
-
     def add_chained_order(self, chained_order):
         """
         chained_order will be assigned with the actually created order when this order will be filled
         warning: add_chained_order is not checking if the order should be created instantly (if self is filled).
         :param chained_order: WrappedOrder to be added to this order's chained orders
         """
         self.chained_orders.append(chained_order)
@@ -425,21 +421,14 @@
         if self.associated_entry_ids is None:
             self.associated_entry_ids = []
         if entry_order_id not in self.associated_entry_ids:
             self.associated_entry_ids.append(entry_order_id)
             return True
         return False
 
-    def replace_associated_entry_id(self, previous_entry_order_id, updated_entry_order_id):
-        if self.associated_entry_ids is None:
-            return
-        for index, entry_id in enumerate(self.associated_entry_ids):
-            if entry_id == previous_entry_order_id:
-                self.associated_entry_ids[index] = updated_entry_order_id
-
     def update_quantity_with_order_fees(self, other_order):
         relevant_fees_amount = order_util.get_fees_for_currency(other_order.fee, self.quantity_currency)
         if relevant_fees_amount:
             logger = logging.get_logger(self.get_logger_name())
             fees_str = f"Paid {self.quantity_currency} fees: {relevant_fees_amount}, " \
                        f"initial order size: {self.origin_quantity}"
             if relevant_fees_amount > self.origin_quantity:
@@ -533,15 +522,15 @@
             else:
                 self.order_profitability = 1 - self.created_last_price / self.filled_price
                 if self.side is enums.TradeOrderSide.BUY:
                     self.order_profitability *= -1
         return self.order_profitability
 
     async def default_exchange_update_order_status(self):
-        raw_order = await self.exchange_manager.exchange.get_order(self.order_id, self.symbol)
+        raw_order = await self.exchange_manager.exchange.get_order(self.exchange_order_id, self.symbol)
         new_status = order_util.parse_order_status(raw_order)
         self.is_synchronized_with_exchange = True
         if new_status in {enums.OrderStatus.FILLED, enums.OrderStatus.CLOSED}:
             await self.on_fill()
         elif new_status is enums.OrderStatus.CANCELED:
             await self.trader.cancel_order(self)
 
@@ -588,15 +577,16 @@
 
         return self.update(
             symbol=str(raw_order.get(enums.ExchangeConstantsOrderColumns.SYMBOL.value, None)),
             current_price=decimal.Decimal(str(price)),
             quantity=decimal.Decimal(str(raw_order.get(enums.ExchangeConstantsOrderColumns.AMOUNT.value, 0.0) or 0.0)),
             price=decimal.Decimal(str(price)),
             status=order_util.parse_order_status(raw_order),
-            order_id=str(raw_order.get(enums.ExchangeConstantsOrderColumns.ID.value, None)),
+            order_id=raw_order.get(enums.ExchangeConstantsOrderColumns.ID.value, None),
+            exchange_order_id=str(raw_order.get(enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value, None)),
             quantity_filled=decimal.Decimal(str(raw_order.get(enums.ExchangeConstantsOrderColumns.FILLED.value, 0.0)
                                                 or 0.0)),
             filled_price=decimal.Decimal(str(filled_price)),
             average_price=decimal.Decimal(str(average_price)),
             total_cost=decimal.Decimal(str(raw_order.get(enums.ExchangeConstantsOrderColumns.COST.value, 0.0) or 0.0)),
             fee=order_util.parse_raw_fees(raw_order.get(enums.ExchangeConstantsOrderColumns.FEE.value, None)),
             timestamp=raw_order.get(enums.ExchangeConstantsOrderColumns.TIMESTAMP.value, None),
@@ -614,14 +604,15 @@
         self.currency = other_order.currency
         self.market = other_order.market
         self.quantity_currency = other_order.quantity_currency
         self.taker_or_maker = other_order.taker_or_maker
         self.side = other_order.side
 
         self.order_id = other_order.order_id
+        self.exchange_order_id = other_order.exchange_order_id
         self.status = other_order.status
 
         self.filled_quantity = other_order.filled_quantity
         self.filled_price = other_order.filled_price
         self.fee = other_order.fee
         self.fees_currency_side = other_order.fees_currency_side
         self.total_cost = other_order.total_cost
@@ -639,20 +630,21 @@
         if other_order.state is not None:
             await other_order.state.replace_order(self)
 
     def update_from_storage_order_details(self, order_details):
         # rebind order attributes that are not stored on exchange
         order_dict = order_details.get(orders_storage.OrdersStorage.ORIGIN_VALUE_KEY, {})
         self.tag = order_dict.get(enums.ExchangeConstantsOrderColumns.TAG.value, self.tag)
+        self.order_id = order_dict.get(enums.ExchangeConstantsOrderColumns.ID.value, self.order_id)
+        self.exchange_order_id = order_dict.get(enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value,
+                                                self.exchange_order_id)
         self.trader_creation_kwargs = order_details.get(enums.StoredOrdersAttr.TRADER_CREATION_KWARGS.value,
                                                         self.trader_creation_kwargs)
         self.exchange_creation_params = order_details.get(enums.StoredOrdersAttr.EXCHANGE_CREATION_PARAMS.value,
                                                           self.exchange_creation_params)
-        self.set_shared_signal_order_id(order_details.get(enums.StoredOrdersAttr.SHARED_SIGNAL_ORDER_ID.value,
-                                                          self.shared_signal_order_id))
         self.has_been_bundled = order_details.get(enums.StoredOrdersAttr.HAS_BEEN_BUNDLED.value,
                                                   self.has_been_bundled)
         self.associated_entry_ids = order_details.get(enums.StoredOrdersAttr.ENTRIES.value,
                                                       self.associated_entry_ids)
         self.update_with_triggering_order_fees = order_details.get(
             enums.StoredOrdersAttr.UPDATE_WITH_TRIGGERING_ORDER_FEES.value, False
         )
@@ -712,23 +704,19 @@
             # always true
             self.taker_or_maker = enums.ExchangeConstantsMarketPropertyColumns.TAKER.value
         else:
             # true 90% of the time: impossible to know for sure the reality
             # (should only be used for simulation anyway)
             self.taker_or_maker = enums.ExchangeConstantsMarketPropertyColumns.MAKER.value
 
-    def ensure_order_id(self):
-        if self.order_id is None and self.is_self_managed():
-            # self managed orders should always have an id, even on real trader
-            self.order_id = order_util.generate_order_id()
-
     def to_dict(self):
         filled_price = self.filled_price if self.filled_price > 0 else self.origin_price
         return {
             enums.ExchangeConstantsOrderColumns.ID.value: self.order_id,
+            enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value: self.exchange_order_id,
             enums.ExchangeConstantsOrderColumns.SYMBOL.value: self.symbol,
             enums.ExchangeConstantsOrderColumns.PRICE.value: filled_price,
             enums.ExchangeConstantsOrderColumns.STATUS.value: self.status.value,
             enums.ExchangeConstantsOrderColumns.TIMESTAMP.value: self.timestamp,
             enums.ExchangeConstantsOrderColumns.TYPE.value: self.exchange_order_type.value
             if self.exchange_order_type else None,
             enums.ExchangeConstantsOrderColumns.SIDE.value: self.side.value,
@@ -758,15 +746,16 @@
         tag = f" | tag: {self.tag}" if self.tag else ""
         return (f"{self.symbol} | "
                 f"{chained_order}"
                 f"{self.order_type.name if self.order_type is not None else 'Unknown'} | "
                 f"Price : {str(self.origin_price)} | "
                 f"Quantity : {str(self.origin_quantity)} | "
                 f"State : {self.state.state.value if self.state is not None else 'Unknown'} | "
-                f"id : {self.order_id}{tag}")
+                f"id : {self.order_id}{tag}"
+                f"exchange id: {self.exchange_order_id}")
 
     def __str__(self):
         return self.to_string()
 
     def is_to_be_maintained(self):
         return self.trader is not None
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/order_adapter.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/order_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/order_factory.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/order_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     symbol,
     current_price,
     quantity,
     price=constants.ZERO,
     stop_price=constants.ZERO,
     status=enums.OrderStatus.OPEN,
     order_id=None,
+    exchange_order_id=None,
     filled_price=constants.ZERO,
     average_price=constants.ZERO,
     quantity_filled=constants.ZERO,
     total_cost=constants.ZERO,
     timestamp=0,
     side=None,
     fees_currency_side=None,
@@ -71,14 +72,15 @@
         order_type=order_type,
         symbol=symbol,
         current_price=current_price,
         quantity=quantity,
         price=price,
         stop_price=stop_price,
         order_id=trader.parse_order_id(order_id),
+        exchange_order_id=exchange_order_id,
         timestamp=timestamp,
         status=status,
         filled_price=filled_price,
         average_price=average_price,
         quantity_filled=quantity_filled,
         fee=None,
         total_cost=total_cost,
@@ -87,15 +89,14 @@
         tag=tag,
         reduce_only=reduce_only,
         quantity_currency=quantity_currency,
         close_position=close_position,
         exchange_creation_params=exchange_creation_params,
         associated_entry_id=associated_entry_id
     )
-    order.ensure_order_id()
     return order
 
 
 def create_order_from_dict(trader, order_dict):
     """
     :param trader: the trader to associate the order to
     :param order_dict: a dict formatted as from order.to_dict()
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/order_group.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/order_state.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/order_util.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/order_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,15 +331,15 @@
             loaded=False,
             params=order.exchange_creation_params,
             **order.trader_creation_kwargs
         )
 
 
 def is_associated_pending_order(pending_order, created_order):
-    return created_order.order_id == pending_order.order_id or (
+    return created_order.exchange_order_id == pending_order.exchange_order_id or (
         created_order.symbol == pending_order.symbol and
         created_order.origin_quantity == pending_order.origin_quantity and
         created_order.origin_price == pending_order.origin_price and
         created_order.__class__ is pending_order.__class__ and
         created_order.trader is pending_order.trader
     )
 
@@ -349,19 +349,21 @@
     if to_be_initialized:
         pending_order.is_initialized = False
     logging.get_logger(LOGGER_NAME).debug(f"Updated pending order: {pending_order} using {created_order}")
 
 
 async def _apply_pending_order_on_existing_orders(pending_order):
     for created_order in pending_order.exchange_manager.exchange_personal_data.orders_manager.get_open_orders(
-            symbol=pending_order.symbol):
+        symbol=pending_order.symbol
+    ):
         if is_associated_pending_order(pending_order, created_order) and created_order.order_group is None:
             await apply_pending_order_from_created_order(pending_order, created_order, False)
-            pending_order.exchange_manager.exchange_personal_data.orders_manager.replace_order(created_order.order_id,
-                                                                                               pending_order)
+            pending_order.exchange_manager.exchange_personal_data.orders_manager.replace_order(
+                created_order.order_id, pending_order
+            )
             created_order.clear()
             return True
     return False
 
 
 @contextlib.asynccontextmanager
 async def ensure_orders_relevancy(order=None, position=None):
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/orders_manager.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/orders_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -74,15 +74,20 @@
         self, symbol=None, since=constants.NO_DATA_LIMIT, until=constants.NO_DATA_LIMIT,
         limit=constants.NO_DATA_LIMIT, tag=None):
         return self._select_orders(
             enums.OrderStatus.CLOSED, symbol, since=since,
             until=until, limit=limit, tag=tag
         )
 
-    def get_order(self, order_id):
+    def get_order(self, order_id, exchange_order_id=None):
+        if order_id is None:
+            for order in self.orders.values():
+                if order.exchange_order_id == exchange_order_id:
+                    return order
+            raise KeyError(exchange_order_id)
         return self.orders[order_id]
 
     def get_order_from_group(self, group_name):
         return [
             order
             for order in self.orders.values()
             if order.order_group is not None and order.order_group.name == group_name
@@ -116,27 +121,28 @@
         if group_name in self.order_groups:
             raise errors.ConflictingOrderGroupError(f"Can't create a new order group named '{group_name}': "
                                                     f"one with this name already exists")
         group = group_type(group_name, self)
         self.order_groups[group_name] = group
         return group
 
-    async def upsert_order_from_raw(self, order_id, raw_order, is_from_exchange) -> bool:
-        if not self.has_order(order_id):
+    async def upsert_order_from_raw(self, exchange_order_id, raw_order, is_from_exchange) -> (bool, order_class.Order):
+        if not self.has_order(None, exchange_order_id=exchange_order_id):
             self.logger.info(f"Including new order fetched from exchange: {raw_order}")
             new_order = order_factory.create_order_instance_from_raw(self.trader, raw_order)
             # replace new_order by previously created pending_order if any relevant pending_order
             new_order = await self.get_and_update_pending_order(new_order) or new_order
             if is_from_exchange:
                 new_order.is_synchronized_with_exchange = True
-            self._add_order(order_id, new_order)
+            self._add_order(new_order.order_id, new_order)
             self._check_orders_size()
             await new_order.initialize(is_from_exchange_data=True)
-            return True
-        return await _update_order_from_raw(self.orders[order_id], raw_order)
+            return True, new_order
+        order = self.get_order(None, exchange_order_id=exchange_order_id)
+        return await _update_order_from_raw(order, raw_order), order
 
     def register_pending_creation_order(self, pending_order):
         if self.trader.simulate:
             self.logger.error(f"Called register_pending_creation_order on an simulated trader, "
                               f"this should not happen. Order: {pending_order}")
         self.pending_creation_orders.append(pending_order)
 
@@ -153,27 +159,27 @@
         for index, pending_order in enumerate(self.pending_creation_orders):
             if order_util.is_associated_pending_order(pending_order, created_order):
                 if should_pop:
                     self.pending_creation_orders.pop(index)
                 return pending_order
         return None
 
-    def get_all_active_and_pending_orders_shared_signal_order_id(self) -> list:
+    def get_all_active_and_pending_orders_id(self) -> list:
         return [
-            order.shared_signal_order_id
+            order.order_id
             for order in self._select_orders()
         ] + [
-            order.shared_signal_order_id
+            order.order_id
             for order in self.pending_creation_orders
         ]
 
-    async def upsert_order_close_from_raw(self, order_id, raw_order) -> typing.Optional[order_class.Order]:
-        if self.has_order(order_id):
-            order = self.orders[order_id]
-            await _update_order_from_raw(self.orders[order_id], raw_order)
+    async def upsert_order_close_from_raw(self, exchange_order_id, raw_order) -> typing.Optional[order_class.Order]:
+        if self.has_order(None, exchange_order_id=exchange_order_id):
+            order = self.get_order(None, exchange_order_id=exchange_order_id)
+            await _update_order_from_raw(order, raw_order)
             return order
         return None
 
     async def upsert_order_instance(self, order) -> bool:
         if not self.has_order(order.order_id):
             # this should not consume pending orders
             if self._get_pending_order(order, False):
@@ -187,15 +193,21 @@
         return False
 
     def _add_order(self, order_id, order):
         if order_id is None:
             self.logger.warning(f"Adding order with None order_id to order manager: {order}")
         self.orders[order_id] = order
 
-    def has_order(self, order_id) -> bool:
+    def has_order(self, order_id, exchange_order_id=None) -> bool:
+        if order_id is None:
+            try:
+                self.get_order(None, exchange_order_id=exchange_order_id)
+                return True
+            except KeyError:
+                return False
         return order_id in set(self.orders.keys())
 
     def remove_order_instance(self, order):
         if self.has_order(order.order_id):
             self.orders.pop(order.order_id, None)
             order.clear()
         else:
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/orders_storage_operations.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/orders_storage_operations.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/states/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/states/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/states/cancel_order_state.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/states/cancel_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/states/close_order_state.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/states/close_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/states/fill_order_state.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/states/fill_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/states/open_order_state.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/states/open_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/states/order_state_factory.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/states/order_state_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/states/pending_creation_chained_order_state.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/states/pending_creation_chained_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/states/pending_creation_order_state.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/states/pending_creation_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/limit/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/limit/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/limit/buy_limit_order.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/limit/buy_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/limit/limit_order.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/limit/limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/limit/sell_limit_order.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/limit/sell_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/limit/stop_loss_order.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/limit/stop_loss_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/limit/take_profit_order.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/limit/take_profit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/market/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/market/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/market/buy_market_order.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/market/buy_market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/market/market_order.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/market/market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/market/sell_market_order.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/market/sell_market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/trailing/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/trailing/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/unknown_order.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/unknown_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/orders/types/unsupported_order.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/orders/types/unsupported_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/asset.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/assets/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/assets/future_asset.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/assets/future_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/assets/margin_asset.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/assets/margin_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/assets/spot_asset.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/assets/spot_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/channel/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/channel/balance.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/channel/balance.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/channel/balance_updater.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/channel/balance_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/history/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/history/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/history/historical_asset_value.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/history/historical_asset_value.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/portfolio.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/portfolio_factory.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/portfolio_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/portfolio_manager.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/portfolio_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/portfolio_profitability.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/portfolio_profitability.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/portfolio_util.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/portfolio_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/portfolio_value_holder.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/portfolio_value_holder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/sub_portfolio.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/sub_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/types/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/types/future_portfolio.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/types/future_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/types/margin_portfolio.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/types/margin_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/types/spot_portfolio.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/types/spot_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/portfolios/value_converter.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/portfolios/value_converter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/channel/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/channel/positions.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/channel/positions.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/channel/positions_updater.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/channel/positions_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/channel/positions_updater_simulator.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/channel/positions_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/position.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/position_factory.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/position_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/position_state.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/position_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/position_util.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/position_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/positions_manager.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/positions_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/states/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/states/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/states/active_position_state.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/states/active_position_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/states/idle_position_state.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/states/idle_position_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/states/liquidate_position_state.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/states/liquidate_position_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/states/position_state_factory.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/states/position_state_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/types/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/types/inverse_position.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/types/inverse_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/positions/types/linear_position.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/positions/types/linear_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/state.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/trades/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/trades/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/trades/channel/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/trades/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/trades/channel/trades.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/trades/channel/trades.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             for trade in trades:
                 if not trade:
                     continue
                 symbol: str = self.channel.exchange_manager.get_exchange_symbol(
                     trade[enums.ExchangeConstantsOrderColumns.SYMBOL.value])
                 if self.channel.get_filtered_consumers(symbol=channel_constants.CHANNEL_WILDCARD) or \
                         self.channel.get_filtered_consumers(symbol=symbol):
-                    trade_id: str = trade[enums.ExchangeConstantsOrderColumns.ID.value]
+                    trade_id: str = trade[enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value]
 
                     await self.channel.exchange_manager.exchange_personal_data.handle_trade_update(
                         symbol,
                         trade_id,
                         trade,
                         is_old_trade=old_trade,
                         should_notify=True)
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/trades/channel/trades_updater.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/trades/channel/trades_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/trades/trade.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/trades/trade.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         self.creation_time = self.exchange_manager.exchange.get_exchange_current_time()
 
         self.trade_id = trader.parse_order_id(None)
         # One order might create multiple trades when matched to multiple open orders.
         # Current implementation creates only one trade per order
         # TODO: update this comment when handling multiple trades per order
         self.origin_order_id = None
+        self.exchange_order_id = None
         self.simulated = True
         self.is_closing_order = False
 
         self.symbol = None
         self.currency = None
         self.market = None
         self.taker_or_maker = None
@@ -75,14 +76,15 @@
         self.quantity_currency = order.quantity_currency
         self.trade_type = order.order_type
         self.exchange_trade_type = order.exchange_order_type
         self.status = order.status
         self.fee = order.fee
         self.trade_id = order.order_id
         self.origin_order_id = order.order_id
+        self.exchange_order_id = order.exchange_order_id
         self.simulated = order.simulated
         self.side = order.side
         self.creation_time = order.creation_time if order.creation_time > 0 else creation_time
         self.canceled_time = order.canceled_time if order.canceled_time > 0 else canceled_time
         self.executed_time = order.executed_time if order.executed_time > 0 else executed_time
         self.symbol = order.symbol
         self.is_closing_order = order.status in self.CLOSING_TRADE_ORDER_STATUS
@@ -99,14 +101,15 @@
     def has_been_executed(self):
         return self.status is not enums.OrderStatus.CANCELED and self.status is not enums.OrderStatus.EXPIRED
 
     def to_dict(self):
         return {
             enums.ExchangeConstantsOrderColumns.ID.value: self.trade_id,
             enums.ExchangeConstantsOrderColumns.ORDER_ID.value: self.origin_order_id,
+            enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value: self.exchange_order_id,
             enums.ExchangeConstantsOrderColumns.SYMBOL.value: self.symbol,
             enums.ExchangeConstantsOrderColumns.MARKET.value: self.market,
             enums.ExchangeConstantsOrderColumns.PRICE.value: self.executed_price,
             enums.ExchangeConstantsOrderColumns.STATUS.value: self.status.value,
             enums.ExchangeConstantsOrderColumns.TIMESTAMP.value: self.get_time(),
             enums.ExchangeConstantsOrderColumns.TYPE.value: self.exchange_trade_type.value,
             enums.ExchangeConstantsOrderColumns.SIDE.value: self.side.value,
@@ -114,21 +117,23 @@
             enums.ExchangeConstantsOrderColumns.COST.value: self.total_cost,
             enums.ExchangeConstantsOrderColumns.QUANTITY_CURRENCY.value: self.quantity_currency,
             enums.ExchangeConstantsOrderColumns.TAKER_OR_MAKER.value: self.taker_or_maker,
             enums.ExchangeConstantsOrderColumns.FEE.value: self.fee,
             enums.ExchangeConstantsOrderColumns.REDUCE_ONLY.value: self.reduce_only,
             enums.ExchangeConstantsOrderColumns.TAG.value: self.tag,
             enums.ExchangeConstantsOrderColumns.ENTRIES.value: self.associated_entry_ids,
+            enums.TradeExtraConstants.CREATION_TIME.value: self.creation_time,
         }
 
     @classmethod
     def from_dict(cls, trader, trade_dict):
         trade = cls(trader)
         trade.trade_id = trade_dict.get(enums.ExchangeConstantsOrderColumns.ID.value)
         trade.origin_order_id = trade_dict.get(enums.ExchangeConstantsOrderColumns.ORDER_ID.value)
+        trade.exchange_order_id = trade_dict.get(enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value)
         trade.symbol = trade_dict.get(enums.ExchangeConstantsOrderColumns.SYMBOL.value)
         trade.currency, trade.market = commons_symbols.parse_symbol(trade.symbol).base_and_quote()
         trade.market = trade_dict.get(enums.ExchangeConstantsOrderColumns.MARKET.value)
         trade.executed_price = decimal.Decimal(str(trade_dict.get(enums.ExchangeConstantsOrderColumns.PRICE.value)))
         trade.status = enums.OrderStatus(trade_dict.get(enums.ExchangeConstantsOrderColumns.STATUS.value,
                                                         enums.OrderStatus.CLOSED.value))
         if trade.has_been_executed():
@@ -151,8 +156,9 @@
         trade.fee = copy.copy(trade_dict.get(enums.ExchangeConstantsOrderColumns.FEE.value))
         if trade.fee and enums.FeePropertyColumns.COST.value in trade.fee:
             trade.fee[enums.FeePropertyColumns.COST.value] = \
                 decimal.Decimal(str(trade.fee[enums.FeePropertyColumns.COST.value]))
         trade.reduce_only = trade_dict.get(enums.ExchangeConstantsOrderColumns.REDUCE_ONLY.value)
         trade.tag = trade_dict.get(enums.ExchangeConstantsOrderColumns.TAG.value)
         trade.associated_entry_ids = trade_dict.get(enums.ExchangeConstantsOrderColumns.ENTRIES.value)
+        trade.creation_time = trade_dict.get(enums.TradeExtraConstants.CREATION_TIME.value)
         return trade
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/trades/trade_factory.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/trades/trade_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,27 +55,29 @@
 
 
 def create_trade_instance(trader,
                           order_type,
                           symbol,
                           status=enums.OrderStatus.CLOSED,
                           order_id=None,
+                          exchange_order_id=None,
                           filled_price=constants.ZERO,
                           quantity_filled=constants.ZERO,
                           total_cost=constants.ZERO,
                           canceled_time=0,
                           creation_time=0,
                           executed_time=0):
     order = order_factory.create_order_from_type(trader=trader, order_type=order_type)
     order.update(order_type=order_type,
                  symbol=symbol,
                  current_price=filled_price,
                  quantity=quantity_filled,
                  price=filled_price,
                  order_id=trader.parse_order_id(order_id),
+                 exchange_order_id=trader.parse_order_id(exchange_order_id),
                  filled_price=filled_price,
                  quantity_filled=quantity_filled,
                  fee=None,  # TODO
                  total_cost=total_cost)
     return create_trade_from_order(order,
                                    close_status=status,
                                    canceled_time=canceled_time,
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/trades/trade_pnl.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/trades/trade_pnl.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/trades/trades_manager.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/trades/trades_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,17 +61,17 @@
         return False
 
     def upsert_trade_instance(self, trade):
         if trade.trade_id not in self.trades:
             self.trades[trade.trade_id] = trade
             self._check_trades_size()
 
-    def has_closing_trade_with_order_id(self, order_id) -> bool:
-        for trade in self.trades.values():
-            if trade.origin_order_id == order_id and trade.is_closing_order:
+    def has_closing_trade_with_exchange_order_id(self, exchange_order_id) -> bool:
+        for trade in self.get_trades(exchange_order_id=exchange_order_id):
+            if trade.is_closing_order:
                 return True
         return False
 
     def get_total_paid_fees(self):
         total_fees = {}
         for trade in self.trades.values():
             if trade.fee is not None:
@@ -82,15 +82,15 @@
                 else:
                     total_fees[fee_currency] = fee_cost
             elif trade.status is not enums.OrderStatus.CANCELED:
                 self.logger.warning(f"Trade without any registered fee: {trade.to_dict()}")
         return total_fees
 
     def get_completed_trades_pnl(self, trades=None) -> list:
-        trades = trades or self.trades.values()
+        trades = trades or self.get_trades()
         trades_by_order_id = {
             trade.origin_order_id: trade
             for trade in trades
         }
         exits_by_entry_id = {}
         for trade in trades:
             if trade.status is not enums.OrderStatus.CANCELED and trade.associated_entry_ids:
@@ -107,14 +107,24 @@
             )
             for entry_id, exit_trade in exits_by_entry_id.items()
         ]
 
     def get_trade(self, trade_id):
         return self.trades[trade_id]
 
+    def get_trades(self, origin_order_id=None, exchange_order_id=None):
+        return [
+            trade
+            for trade in self.trades.values()
+            if (
+                (not origin_order_id or trade.origin_order_id == origin_order_id)
+                and (not exchange_order_id or trade.exchange_order_id == exchange_order_id)
+            )
+        ]
+
     # private
     def _check_trades_size(self):
         if len(self.trades) > self.MAX_TRADES_COUNT:
             self._remove_oldest_trades(int(self.MAX_TRADES_COUNT / 10))
 
     def _reset_trades(self):
         self.trades_initialized = False
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/trades/trades_util.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/trades/trades_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/transactions/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/transactions/transaction.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/transactions/transaction_factory.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/transactions/transaction_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/transactions/transactions_manager.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/transactions/transactions_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/transactions/types/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/transactions/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/transactions/types/blockchain_transaction.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/transactions/types/blockchain_transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/transactions/types/fee_transaction.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/transactions/types/fee_transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/personal_data/transactions/types/transfer_transaction.py` & `OctoBot-Trading-2.4.3/octobot_trading/personal_data/transactions/types/transfer_transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/signals/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/signals/channel/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/signals/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/signals/channel/remote_trading_signal.py` & `OctoBot-Trading-2.4.3/octobot_trading/signals/channel/remote_trading_signal.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/signals/channel/remote_trading_signal_channel_factory.py` & `OctoBot-Trading-2.4.3/octobot_trading/signals/channel/remote_trading_signal_channel_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/signals/channel/signal_producer.py` & `OctoBot-Trading-2.4.3/octobot_trading/signals/channel/signal_producer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/signals/signal_creation.py` & `OctoBot-Trading-2.4.3/octobot_trading/signals/signal_creation.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,35 +56,50 @@
 def should_emit_trading_signal(exchange_manager):
     try:
         return exchange_manager.trading_modes[0].should_emit_trading_signal()
     except IndexError:
         return False
 
 
+async def _get_order_portfolio_percent(order, exchange_manager):
+    percent = await orders.get_order_size_portfolio_percent(
+        exchange_manager,
+        order.origin_quantity,
+        order.side,
+        order.symbol
+    )
+    return f"{float(percent)}{script_keywords.QuantityType.PERCENT.value}"
+
+
 async def create_order(exchange_manager, should_emit_signal, order,
                        loaded: bool = False, params: dict = None,
                        wait_for_creation=True,
                        creation_timeout=constants.INDIVIDUAL_ORDER_SYNC_TIMEOUT):
     order_pf_percent = f"0{script_keywords.QuantityType.PERCENT.value}"
+    chained_orders_pf_percent = []
     if should_emit_signal:
-        percent = await orders.get_order_size_portfolio_percent(
-            exchange_manager,
-            order.origin_quantity,
-            order.side,
-            order.symbol
-        )
-        order_pf_percent = f"{float(percent)}{script_keywords.QuantityType.PERCENT.value}"
+        order_pf_percent = await _get_order_portfolio_percent(order, exchange_manager)
+        chained_orders_pf_percent = [
+            (chained_order, await _get_order_portfolio_percent(chained_order, exchange_manager))
+            for chained_order in order.chained_orders
+        ]
     created_order = await exchange_manager.trader.create_order(
         order, loaded=loaded, params=params,
         wait_for_creation=wait_for_creation, creation_timeout=creation_timeout
     )
     if created_order is not None and should_emit_signal:
-        signals.SignalPublisher.instance().get_signal_bundle_builder(order.symbol).add_created_order(
+        builder = signals.SignalPublisher.instance().get_signal_bundle_builder(order.symbol)
+        builder.add_created_order(
             created_order, exchange_manager, target_amount=order_pf_percent
         )
+        for chained_order, chained_order_pf_percent in chained_orders_pf_percent:
+            builder.add_created_order(
+                chained_order, exchange_manager, target_amount=chained_order_pf_percent
+            )
+
     return created_order
 
 
 async def cancel_order(exchange_manager, should_emit_signal, order, ignored_order: object = None,
                        wait_for_cancelling=True, cancelling_timeout=constants.INDIVIDUAL_ORDER_SYNC_TIMEOUT) -> bool:
     cancelled = await exchange_manager.trader.cancel_order(
         order, ignored_order=ignored_order,
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/signals/trading_signal_bundle_builder.py` & `OctoBot-Trading-2.4.3/octobot_trading/signals/trading_signal_bundle_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         updated_target_amount=None,
         updated_target_position=None,
         updated_limit_price=trading_constants.ZERO,
         updated_stop_price=trading_constants.ZERO,
         updated_current_price=trading_constants.ZERO,
     ):
         try:
-            index, order_description = self._get_order_description_from_local_orders(order.shared_signal_order_id)
+            index, order_description = self._get_order_description_from_local_orders(order.order_id)
             if action is trading_enums.TradingSignalOrdersActions.CREATE:
                 # replace order
                 self.signals[index] = self.create_signal(
                     trading_enums.TradingSignalTopics.ORDERS.value,
                     signal_util.create_order_signal_content(
                         order,
                         trading_enums.TradingSignalOrdersActions.CREATE,
@@ -212,15 +212,14 @@
                     include_signal = False
                 else:
                     order_description_by_seen_group_ids[add_to_group_ids] = signal.content
             if include_signal:
                 filtered_signals.append(signal)
         self.signals = filtered_signals
 
-    def _get_order_description_from_local_orders(self, shared_signal_order_id):
+    def _get_order_description_from_local_orders(self, order_id):
         for index, signal in enumerate(self.signals):
-            if signal.content[trading_enums.TradingSignalOrdersAttrs.SHARED_SIGNAL_ORDER_ID.value] == \
-                    shared_signal_order_id:
+            if signal.content[trading_enums.TradingSignalOrdersAttrs.ORDER_ID.value] == order_id:
                 return index, signal.content
         raise trading_errors.OrderDescriptionNotFoundError(
-            f"order not found (shared_signal_order_id: {shared_signal_order_id})"
+            f"order not found (order_id: {order_id})"
         )
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/signals/util.py` & `OctoBot-Trading-2.4.3/octobot_trading/signals/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         target_position=None,
         updated_target_amount=None,
         updated_target_position=None,
         updated_limit_price=trading_constants.ZERO,
         updated_stop_price=trading_constants.ZERO,
         updated_current_price=trading_constants.ZERO,
 ) -> dict:
+    # only use order.order_id to identify orders in signals (exchange_order_id is local and never shared)
     return {
         trading_enums.TradingSignalCommonsAttrs.ACTION.value: action.value,
         trading_enums.TradingSignalOrdersAttrs.STRATEGY.value: strategy,
         trading_enums.TradingSignalOrdersAttrs.SYMBOL.value: order.symbol,
         trading_enums.TradingSignalOrdersAttrs.EXCHANGE.value: exchange_manager.exchange_name,
         trading_enums.TradingSignalOrdersAttrs.EXCHANGE_TYPE.value: exchanges.get_exchange_type(exchange_manager).value,
         trading_enums.TradingSignalOrdersAttrs.SIDE.value: order.side.value,
@@ -56,15 +57,15 @@
         trading_enums.TradingSignalOrdersAttrs.POST_ONLY.value: False,
         trading_enums.TradingSignalOrdersAttrs.GROUP_ID.value:
             None if order.order_group is None else order.order_group.name,
         trading_enums.TradingSignalOrdersAttrs.GROUP_TYPE.value:
             None if order.order_group is None else order.order_group.__class__.__name__,
         trading_enums.TradingSignalOrdersAttrs.TAG.value: order.tag,
         trading_enums.TradingSignalOrdersAttrs.ASSOCIATED_ORDER_IDS.value: order.associated_entry_ids,
-        trading_enums.TradingSignalOrdersAttrs.SHARED_SIGNAL_ORDER_ID.value: order.shared_signal_order_id,
+        trading_enums.TradingSignalOrdersAttrs.ORDER_ID.value: order.order_id,
         trading_enums.TradingSignalOrdersAttrs.BUNDLED_WITH.value:
-            None if order.triggered_by is None else order.triggered_by.shared_signal_order_id
+            None if order.triggered_by is None else order.triggered_by.order_id
         if order.has_been_bundled else None,
         trading_enums.TradingSignalOrdersAttrs.CHAINED_TO.value:
-            None if order.triggered_by is None else order.triggered_by.shared_signal_order_id,
+            None if order.triggered_by is None else order.triggered_by.order_id,
         trading_enums.TradingSignalOrdersAttrs.ADDITIONAL_ORDERS.value: [],
     }
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/storage/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/storage/abstract_storage.py` & `OctoBot-Trading-2.4.3/octobot_trading/storage/abstract_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/storage/candles_storage.py` & `OctoBot-Trading-2.4.3/octobot_trading/storage/candles_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/storage/orders_storage.py` & `OctoBot-Trading-2.4.3/octobot_trading/storage/orders_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,14 @@
     try:
         return {
             OrdersStorage.ORIGIN_VALUE_KEY: OrdersStorage.sanitize_for_storage(order.to_dict()),
             enums.StoredOrdersAttr.EXCHANGE_CREATION_PARAMS.value:
                 OrdersStorage.sanitize_for_storage(order.exchange_creation_params),
             enums.StoredOrdersAttr.TRADER_CREATION_KWARGS.value:
                 OrdersStorage.sanitize_for_storage(order.trader_creation_kwargs),
-            enums.StoredOrdersAttr.SHARED_SIGNAL_ORDER_ID.value: order.shared_signal_order_id,
             enums.StoredOrdersAttr.HAS_BEEN_BUNDLED.value: order.has_been_bundled,
             enums.StoredOrdersAttr.ENTRIES.value: order.associated_entry_ids,
             enums.StoredOrdersAttr.GROUP.value: _get_group_dict(order),
             enums.StoredOrdersAttr.CHAINED_ORDERS.value:
                 _get_chained_orders(order, exchange_manager),
             enums.StoredOrdersAttr.UPDATE_WITH_TRIGGERING_ORDER_FEES.value:
                 order.update_with_triggering_order_fees,
@@ -206,17 +205,15 @@
         enums.StoredOrdersAttr.ORDER_STATUS.value: status,
         enums.StoredOrdersAttr.UPDATE_TIME.value: update_time,
         enums.StoredOrdersAttr.UPDATE_TYPE.value: update_type,
     }
     details = None
     try:
         details = _format_order(
-            exchange_manager.exchange_personal_data.orders_manager.get_order(
-                order_dict[enums.ExchangeConstantsOrderColumns.ID.value]
-            ),
+            exchange_manager.exchange_personal_data.orders_manager.get_order(order_id),
             exchange_manager
         )
     except KeyError:
         if status == enums.OrderStatus.OPEN.value:
             # ensure order details are present in open orders
             details = {
                 OrdersStorage.ORIGIN_VALUE_KEY: OrdersStorage.sanitize_for_storage(order_dict),
```

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/storage/portfolio_storage.py` & `OctoBot-Trading-2.4.3/octobot_trading/storage/portfolio_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/storage/storage_manager.py` & `OctoBot-Trading-2.4.3/octobot_trading/storage/storage_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/storage/trades_storage.py` & `OctoBot-Trading-2.4.3/octobot_trading/storage/trades_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/storage/transactions_storage.py` & `OctoBot-Trading-2.4.3/octobot_trading/storage/transactions_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/storage/util.py` & `OctoBot-Trading-2.4.3/octobot_trading/storage/util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/supervisors/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/supervisors/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/supervisors/abstract_portfolio_supervisor.py` & `OctoBot-Trading-2.4.3/octobot_trading/supervisors/abstract_portfolio_supervisor.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/supervisors/abstract_supervisor.py` & `OctoBot-Trading-2.4.3/octobot_trading/supervisors/abstract_supervisor.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/util/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/util/config_util.py` & `OctoBot-Trading-2.4.3/octobot_trading/util/config_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/util/initializable.py` & `OctoBot-Trading-2.4.3/octobot_trading/util/initializable.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/util/initialization_util.py` & `OctoBot-Trading-2.4.3/octobot_trading/util/initialization_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/util/simulator_updater_utils.py` & `OctoBot-Trading-2.4.3/octobot_trading/util/simulator_updater_utils.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/util/test_tools/__init__.py` & `OctoBot-Trading-2.4.3/octobot_trading/util/test_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/util/test_tools/exchanges_test_tools.py` & `OctoBot-Trading-2.4.3/octobot_trading/util/test_tools/exchanges_test_tools.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py` & `OctoBot-Trading-2.4.3/octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/octobot_trading/util/test_tools/websocket_test_tools.py` & `OctoBot-Trading-2.4.3/octobot_trading/util/test_tools/websocket_test_tools.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/requirements.txt` & `OctoBot-Trading-2.4.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/setup.py` & `OctoBot-Trading-2.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/api/__init__.py` & `OctoBot-Trading-2.4.3/tests/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/api/test_channels.py` & `OctoBot-Trading-2.4.3/tests/api/test_channels.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/api/test_exchange.py` & `OctoBot-Trading-2.4.3/tests/api/test_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/api/test_modes.py` & `OctoBot-Trading-2.4.3/tests/api/test_modes.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/api/test_orders.py` & `OctoBot-Trading-2.4.3/tests/api/test_orders.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/api/test_portfolio.py` & `OctoBot-Trading-2.4.3/tests/api/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/api/test_profitability.py` & `OctoBot-Trading-2.4.3/tests/api/test_profitability.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/api/test_symbol_data.py` & `OctoBot-Trading-2.4.3/tests/api/test_symbol_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/api/test_trader.py` & `OctoBot-Trading-2.4.3/tests/api/test_trader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/api/test_trades.py` & `OctoBot-Trading-2.4.3/tests/api/test_trades.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/cli/__init__.py` & `OctoBot-Trading-2.4.3/tests/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/__init__.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/contracts/__init__.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/contracts/test_future_contract.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/contracts/test_future_contract.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/contracts/test_margin_contract.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/contracts/test_margin_contract.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/funding/__init__.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/funding/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/funding/test_funding_manager.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/funding/test_funding_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/kline/__init__.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/kline/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/kline/test_kline_manager.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/kline/test_kline_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/ohlcv/__init__.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/ohlcv/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/ohlcv/test_candles_adapter.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/ohlcv/test_candles_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/ohlcv/test_candles_manager.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/ohlcv/test_candles_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/order_book/__init__.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/order_book/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/order_book/test_order_book_manager.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/order_book/test_order_book_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/prices/__init__.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/prices/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/prices/test_price_events_manager.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/prices/test_price_events_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/prices/test_prices_manager.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/prices/test_prices_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/recent_trades/__init__.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/recent_trades/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/recent_trades/test_recent_trades_manager.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/recent_trades/test_recent_trades_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/test_exchange_symbols_data.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/test_exchange_symbols_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/ticker/__init__.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/ticker/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchange_data/ticker/test_ticker_manager.py` & `OctoBot-Trading-2.4.3/tests/exchange_data/ticker/test_ticker_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/__init__.py` & `OctoBot-Trading-2.4.3/tests/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/connectors/__init__.py` & `OctoBot-Trading-2.4.3/tests/exchanges/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/connectors/ccxt/test_ccxt_connector.py` & `OctoBot-Trading-2.4.3/tests/exchanges/connectors/ccxt/test_ccxt_connector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/implementations/__init__.py` & `OctoBot-Trading-2.4.3/tests/exchanges/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/implementations/test_default_rest_exchange.py` & `OctoBot-Trading-2.4.3/tests/exchanges/implementations/test_default_rest_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/implementations/test_default_websocket_exchange.py` & `OctoBot-Trading-2.4.3/tests/exchanges/implementations/test_default_websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/test_abstract_exchange.py` & `OctoBot-Trading-2.4.3/tests/exchanges/test_abstract_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/test_abstract_websocket_exchange.py` & `OctoBot-Trading-2.4.3/tests/exchanges/test_abstract_websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/test_basic_exchange_wrapper.py` & `OctoBot-Trading-2.4.3/tests/exchanges/test_basic_exchange_wrapper.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/test_exchange_builder.py` & `OctoBot-Trading-2.4.3/tests/exchanges/test_exchange_builder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/test_exchange_config_data.py` & `OctoBot-Trading-2.4.3/tests/exchanges/test_exchange_config_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/test_exchange_factory.py` & `OctoBot-Trading-2.4.3/tests/exchanges/test_exchange_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/test_exchange_manager.py` & `OctoBot-Trading-2.4.3/tests/exchanges/test_exchange_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/test_exchange_simulator.py` & `OctoBot-Trading-2.4.3/tests/exchanges/test_exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/test_exchanges.py` & `OctoBot-Trading-2.4.3/tests/exchanges/test_exchanges.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/traders/__init__.py` & `OctoBot-Trading-2.4.3/tests/exchanges/traders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/traders/test_trader.py` & `OctoBot-Trading-2.4.3/tests/exchanges/traders/test_trader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/types/__init__.py` & `OctoBot-Trading-2.4.3/tests/exchanges/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/types/test_websocket_exchange.py` & `OctoBot-Trading-2.4.3/tests/exchanges/types/test_websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/util/__init__.py` & `OctoBot-Trading-2.4.3/tests/exchanges/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/util/test_exchange_market_status_fixer.py` & `OctoBot-Trading-2.4.3/tests/exchanges/util/test_exchange_market_status_fixer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/exchanges/util/test_exchange_util.py` & `OctoBot-Trading-2.4.3/tests/exchanges/util/test_exchange_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/modes/__init__.py` & `OctoBot-Trading-2.4.3/tests/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/modes/script_keywords/__init__.py` & `OctoBot-Trading-2.4.3/tests/modes/script_keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/modes/script_keywords/basic_keywords/test_account_balance.py` & `OctoBot-Trading-2.4.3/tests/modes/script_keywords/basic_keywords/test_account_balance.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/modes/script_keywords/basic_keywords/test_amount.py` & `OctoBot-Trading-2.4.3/tests/modes/script_keywords/basic_keywords/test_amount.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/modes/script_keywords/dsl/__init__.py` & `OctoBot-Trading-2.4.3/tests/modes/script_keywords/dsl/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/modes/script_keywords/dsl/test_quantity.py` & `OctoBot-Trading-2.4.3/tests/modes/script_keywords/dsl/test_quantity.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/modes/test_abstract_mode_consumer.py` & `OctoBot-Trading-2.4.3/tests/modes/test_abstract_mode_consumer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/modes/test_abstract_trading_mode.py` & `OctoBot-Trading-2.4.3/tests/modes/test_abstract_trading_mode.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/__init__.py` & `OctoBot-Trading-2.4.3/tests/personal_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/__init__.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/groups/__init__.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/groups/test_balanced_take_profit_and_stop_order_group.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/groups/test_balanced_take_profit_and_stop_order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/groups/test_group_util.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/groups/test_group_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/groups/test_one_cancels_the_other_order_group.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/groups/test_one_cancels_the_other_order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/states/__init__.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/states/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/states/test_cancel_order_state.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/states/test_cancel_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/states/test_close_order_state.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/states/test_close_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/states/test_fill_order_state.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/states/test_fill_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/states/test_open_order_state.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/states/test_open_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/states/test_order_state.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/states/test_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/states/test_order_state_factory.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/states/test_order_state_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/states/test_pending_creation_chained_order_state.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/states/test_pending_creation_chained_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/states/test_pending_creation_order_state.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/states/test_pending_creation_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/test_decimal_order_adapter.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/test_decimal_order_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/test_double_filled_order.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/test_double_filled_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/test_order.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/test_order.py`

 * *Files 6% similar despite different names*

```diff
@@ -167,14 +167,15 @@
 
 async def test_update_from_raw(trader_simulator):
     config, exchange_manager_inst, trader_inst = trader_simulator
     order_inst = personal_data.Order(trader_inst)
     # binance example market order
     raw_order = {
         'id': '362550114',
+        'exchange_id': '123',
         'clientOrderId': 'x-T9698eeeeeeeeeeeeee792',
         'timestamp': 1637579281.377,
         'datetime': '2021-11-22T11:08:01.377Z',
         'lastTradeTimestamp': None,
         'symbol': 'UNI/USDT',
         'type': 'market',
         'timeInForce': 'GTC',
@@ -191,14 +192,15 @@
         'fee': {'cost': 0.03764836, 'currency': 'USDT'},
         'trades': [],
         'fees': []
     }
     assert order_inst.update_from_raw(raw_order) is True
     assert order_inst.order_type is enums.TraderOrderType.SELL_MARKET
     assert order_inst.order_id == "362550114"
+    assert order_inst.exchange_order_id == "123"
     assert order_inst.side is enums.TradeOrderSide.SELL
     assert order_inst.status is enums.OrderStatus.CLOSED
     assert order_inst.symbol == "UNI/USDT"
     assert order_inst.currency == "UNI"
     assert order_inst.market == "USDT"
     assert order_inst.taker_or_maker is enums.ExchangeConstantsMarketPropertyColumns.TAKER.value
     assert order_inst.origin_price == constants.ZERO
@@ -217,14 +219,15 @@
         enums.FeePropertyColumns.IS_FROM_EXCHANGE.value: True,
     }
 
     order_inst = personal_data.Order(trader_inst)
     # binance example limit order
     raw_order = {
         'id': '362550114',
+        'exchange_id': '123a',
         'clientOrderId': 'x-T9698eeeeeeeeeeeeee792',
         'timestamp': 1637579281.377,
         'datetime': '2021-11-22T11:08:01.377Z',
         'lastTradeTimestamp': None,
         'symbol': 'UNI/USDT',
         'type': 'limit',
         'timeInForce': 'GTC',
@@ -241,14 +244,15 @@
         'fee': {'cost': 0.03764836, 'currency': 'USDT'},
         'trades': [],
         'fees': []
     }
     assert order_inst.update_from_raw(raw_order) is True
     assert order_inst.order_type is enums.TraderOrderType.BUY_LIMIT
     assert order_inst.order_id == "362550114"
+    assert order_inst.exchange_order_id == "123a"
     assert order_inst.side is enums.TradeOrderSide.BUY
     assert order_inst.status is enums.OrderStatus.CLOSED
     assert order_inst.symbol == "UNI/USDT"
     assert order_inst.currency == "UNI"
     assert order_inst.market == "USDT"
     assert order_inst.taker_or_maker is enums.ExchangeConstantsMarketPropertyColumns.MAKER.value
     assert order_inst.origin_price == decimal.Decimal("12.664")
@@ -316,97 +320,107 @@
 
 
 async def test_update_from_order(trader_simulator):
     config, exchange_manager_inst, trader_inst = trader_simulator
 
     base_order_1 = personal_data.Order(trader_inst)
     base_order_1.order_id = "1"
+    base_order_1.exchange_order_id = "1a"
     base_order_1.status = enums.OrderStatus.OPEN
     base_order_1.filled_price = decimal.Decimal("2")
 
     base_order_2 = personal_data.Order(trader_inst)
     base_order_2.order_id = "2"
+    base_order_2.exchange_order_id = "2a"
     base_order_2.status = enums.OrderStatus.CLOSED
     base_order_2.filled_price = decimal.Decimal("3")
 
     # no state
     await base_order_1.update_from_order(base_order_2)
     assert base_order_1.order_id == "2"
+    assert base_order_1.exchange_order_id == "2a"
     assert base_order_1.status == enums.OrderStatus.CLOSED
     assert base_order_1.filled_price == decimal.Decimal("3")
 
     # with state
     state_1 = personal_data.OpenOrderState(base_order_1, False)
     state_2 = personal_data.OpenOrderState(base_order_2, False)
     base_order_1.state = state_1
     base_order_2.state = state_2
     base_order_2.order_id = "3"
+    base_order_2.exchange_order_id = "3AAAAA"
     base_order_2.status = enums.OrderStatus.CANCELED
     base_order_2.filled_price = decimal.Decimal("4")
     await base_order_1.update_from_order(base_order_2)
     assert base_order_1.order_id == "3"
+    assert base_order_1.exchange_order_id == "3AAAAA"
     assert base_order_1.status == enums.OrderStatus.CANCELED
     assert base_order_1.filled_price == decimal.Decimal("4")
     assert base_order_1.state is state_2
     assert base_order_1.state.order is base_order_1
 
 
 async def test_update_from_order_storage(trader_simulator):
     config, exchange_manager_inst, trader_inst = trader_simulator
 
     order = personal_data.BuyLimitOrder(trader_inst)
     order.update(order_type=enums.TraderOrderType.BUY_LIMIT,
                  symbol="BTC/USDT",
                  current_price=decimal.Decimal("70"),
                  quantity=decimal.Decimal("10"),
-                 price=decimal.Decimal("70"))
+                 price=decimal.Decimal("70"),
+                 exchange_order_id="PLOP")
     origin_tag = order.tag
     origin_trader_creation_kwargs = order.trader_creation_kwargs
     origin_exchange_creation_params = order.exchange_creation_params
-    origin_shared_signal_order_id = order.shared_signal_order_id
+    origin_order_id = order.order_id
+    origin_exchange_order_id = order.exchange_order_id
     origin_has_been_bundled = order.has_been_bundled
     origin_associated_entry_ids = order.associated_entry_ids
     origin_update_with_triggering_order_fees = order.update_with_triggering_order_fees
 
     # wrong format
     order.update_from_storage_order_details({"hello": "hi there"})
     assert order.tag is origin_tag
     assert order.trader_creation_kwargs is origin_trader_creation_kwargs
     assert order.exchange_creation_params is origin_exchange_creation_params
-    assert order.shared_signal_order_id is origin_shared_signal_order_id
+    assert order.order_id is origin_order_id
+    assert order.exchange_order_id is origin_exchange_order_id
     assert order.has_been_bundled is origin_has_been_bundled
     assert order.associated_entry_ids is origin_associated_entry_ids
     assert order.update_with_triggering_order_fees is origin_update_with_triggering_order_fees
 
     # partial update
     order.update_from_storage_order_details({
-        enums.StoredOrdersAttr.TRADER_CREATION_KWARGS.value: {"plop": 1},
-        enums.StoredOrdersAttr.SHARED_SIGNAL_ORDER_ID.value: "11"
+        enums.StoredOrdersAttr.TRADER_CREATION_KWARGS.value: {"plop": 1}
     })
     assert order.tag is origin_tag
     assert order.trader_creation_kwargs == {"plop": 1} != origin_trader_creation_kwargs
     assert order.exchange_creation_params is origin_exchange_creation_params
-    assert order.shared_signal_order_id == "11" != origin_shared_signal_order_id
+    assert order.order_id is origin_order_id
+    assert order.exchange_order_id is origin_exchange_order_id
     assert order.has_been_bundled is origin_has_been_bundled
     assert order.associated_entry_ids is origin_associated_entry_ids
     assert order.update_with_triggering_order_fees is origin_update_with_triggering_order_fees
 
     # full update
     order.update_from_storage_order_details({
         orders_storage.OrdersStorage.ORIGIN_VALUE_KEY: {
             enums.ExchangeConstantsOrderColumns.TAG.value: "t1",
+            enums.ExchangeConstantsOrderColumns.ID.value: "11a",
+            enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value: "eee1",
         },
         enums.StoredOrdersAttr.TRADER_CREATION_KWARGS.value: {"plop2": 1},
         enums.StoredOrdersAttr.EXCHANGE_CREATION_PARAMS.value: {"ex": 2, "gg": "yesyes"},
-        enums.StoredOrdersAttr.SHARED_SIGNAL_ORDER_ID.value: "11a",
         enums.StoredOrdersAttr.HAS_BEEN_BUNDLED.value: True,
         enums.StoredOrdersAttr.ENTRIES.value: ["ABC", "2"],
         enums.StoredOrdersAttr.UPDATE_WITH_TRIGGERING_ORDER_FEES.value: True,
     })
     assert order.tag == "t1" != origin_tag
     assert order.trader_creation_kwargs == {"plop2": 1} != origin_trader_creation_kwargs
     assert order.exchange_creation_params == {"ex": 2, "gg": "yesyes"} != origin_exchange_creation_params
-    assert order.shared_signal_order_id == "11a" != origin_shared_signal_order_id
+    assert order.order_id == "11a" != origin_order_id
+    assert order.exchange_order_id == "eee1" != origin_exchange_order_id
     assert order.has_been_bundled is True is not origin_has_been_bundled
     assert order.associated_entry_ids == ["ABC", "2"] != origin_associated_entry_ids
     assert order.has_been_bundled is True is not origin_has_been_bundled
     assert order.update_with_triggering_order_fees is True is not origin_update_with_triggering_order_fees
```

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/test_order_adapter.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/test_order_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/test_order_factory.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/test_order_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/test_order_util.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/test_order_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/test_orders_manager.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/test_orders_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/test_orders_storage_operations.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/test_orders_storage_operations.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import mock
 import pytest
 import pytest_asyncio
 import decimal
 
 import octobot_trading.enums as enums
 import octobot_trading.personal_data as personal_data
+import octobot_trading.storage as storage
 
 from tests import event_loop
 from tests.exchanges import exchange_manager, simulated_exchange_manager
 from tests.exchanges.traders import trader_simulator
 from tests.exchanges.traders import trader
 
 # All test coroutines will be treated as marked.
@@ -61,14 +62,19 @@
 
     # ensure no crash with not well formatted order_details
     mocked_order_storage.get_startup_order_details = mock.AsyncMock(return_value={"hello": "hi there"})
     await personal_data.apply_order_storage_details_if_any(order, exchange_manager_inst, {})
     mocked_order_storage.get_startup_order_details.assert_awaited_once()
 
     # ensure order update is done
-    assert order.shared_signal_order_id != "new id 123"
+    assert order.order_id != "new id 123"
+    assert order.exchange_order_id != "new exchange id 123"
     mocked_order_storage.get_startup_order_details = mock.AsyncMock(return_value={
-        enums.StoredOrdersAttr.SHARED_SIGNAL_ORDER_ID.value: "new id 123"
+        storage.OrdersStorage.ORIGIN_VALUE_KEY: {
+            enums.ExchangeConstantsOrderColumns.ID.value: "new id 123",
+            enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value: "new exchange id 123"
+        }
     })
     await personal_data.apply_order_storage_details_if_any(order, exchange_manager_inst, {})
     mocked_order_storage.get_startup_order_details.assert_awaited_once()
-    assert order.shared_signal_order_id == "new id 123"
+    assert order.order_id == "new id 123"
+    assert order.exchange_order_id == "new exchange id 123"
```

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/types/__init__.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/types/limit/test_buy_limit_order.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/types/limit/test_buy_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/types/limit/test_sell_limit_order.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/types/limit/test_sell_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/types/limit/test_stop_loss_order.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/types/limit/test_stop_loss_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/types/limit/test_take_profit_limit_order.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/types/limit/test_take_profit_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/types/limit/test_take_profit_order.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/types/limit/test_take_profit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/types/market/test_buy_market_order.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/types/market/test_buy_market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/types/market/test_sell_market_order.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/types/market/test_sell_market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/types/test_unknown_order.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/types/test_unknown_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/types/trailing/__init__.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/types/trailing/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/types/trailing/test_trailing_stop_limit_order.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/types/trailing/test_trailing_stop_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/orders/types/trailing/test_trailing_stop_order.py` & `OctoBot-Trading-2.4.3/tests/personal_data/orders/types/trailing/test_trailing_stop_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/portfolios/__init__.py` & `OctoBot-Trading-2.4.3/tests/personal_data/portfolios/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/portfolios/assets/__init__.py` & `OctoBot-Trading-2.4.3/tests/personal_data/portfolios/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/portfolios/assets/test_future_asset.py` & `OctoBot-Trading-2.4.3/tests/personal_data/portfolios/assets/test_future_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/portfolios/assets/test_margin_asset.py` & `OctoBot-Trading-2.4.3/tests/personal_data/portfolios/assets/test_margin_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/portfolios/assets/test_spot_asset.py` & `OctoBot-Trading-2.4.3/tests/personal_data/portfolios/assets/test_spot_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/portfolios/history/test_historical_asset_value_factory.py` & `OctoBot-Trading-2.4.3/tests/personal_data/portfolios/history/test_historical_asset_value_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/portfolios/history/test_historical_portfolio_value_manager.py` & `OctoBot-Trading-2.4.3/tests/personal_data/portfolios/history/test_historical_portfolio_value_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/portfolios/test_asset.py` & `OctoBot-Trading-2.4.3/tests/personal_data/portfolios/test_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/portfolios/test_portfolio.py` & `OctoBot-Trading-2.4.3/tests/personal_data/portfolios/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/portfolios/test_portfolio_manager.py` & `OctoBot-Trading-2.4.3/tests/personal_data/portfolios/test_portfolio_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/portfolios/test_portfolio_profitability.py` & `OctoBot-Trading-2.4.3/tests/personal_data/portfolios/test_portfolio_profitability.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/portfolios/test_portfolio_value_holder.py` & `OctoBot-Trading-2.4.3/tests/personal_data/portfolios/test_portfolio_value_holder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/portfolios/test_value_converter.py` & `OctoBot-Trading-2.4.3/tests/personal_data/portfolios/test_value_converter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/portfolios/types/__init__.py` & `OctoBot-Trading-2.4.3/tests/personal_data/portfolios/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/portfolios/types/test_future_portfolio.py` & `OctoBot-Trading-2.4.3/tests/personal_data/portfolios/types/test_future_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/portfolios/types/test_margin_portfolio.py` & `OctoBot-Trading-2.4.3/tests/personal_data/portfolios/types/test_margin_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/portfolios/types/test_spot_portfolio.py` & `OctoBot-Trading-2.4.3/tests/personal_data/portfolios/types/test_spot_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/positions/__init__.py` & `OctoBot-Trading-2.4.3/tests/personal_data/positions/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/positions/channel/__init__.py` & `OctoBot-Trading-2.4.3/tests/personal_data/positions/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/positions/states/__init__.py` & `OctoBot-Trading-2.4.3/tests/personal_data/positions/states/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/positions/test_position.py` & `OctoBot-Trading-2.4.3/tests/personal_data/positions/test_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/positions/test_position_factory.py` & `OctoBot-Trading-2.4.3/tests/personal_data/positions/test_position_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/positions/test_positions_manager.py` & `OctoBot-Trading-2.4.3/tests/personal_data/positions/test_positions_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/positions/types/__init__.py` & `OctoBot-Trading-2.4.3/tests/personal_data/positions/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/positions/types/test_inverse_position.py` & `OctoBot-Trading-2.4.3/tests/personal_data/positions/types/test_inverse_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/positions/types/test_linear_position.py` & `OctoBot-Trading-2.4.3/tests/personal_data/positions/types/test_linear_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/trades/__init__.py` & `OctoBot-Trading-2.4.3/tests/personal_data/trades/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import octobot_trading.personal_data as personal_data
 
 
-def create_trade(trader, trade_id, is_closing_order, origin_order_id):
+def create_trade(trader, exchange_order_id, is_closing_order, origin_order_id):
     trade = personal_data.Trade(trader)
-    trade.trade_id = trade_id
+    trade.exchange_order_id = exchange_order_id
     trade.is_closing_order = is_closing_order
     trade.origin_order_id = origin_order_id
     return trade
 
 
 def create_executed_trade(trader, side, executed_time, executed_quantity, executed_price, symbol, fee):
     trade = personal_data.Trade(trader)
```

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/trades/test_trade_factory.py` & `OctoBot-Trading-2.4.3/tests/personal_data/trades/test_trade_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         _, exchange_manager, trader = await self.init_default()
 
         raw_trade = json.loads(
             """
             {	
               "info": {},
               "id": "12345-67890:09876/54321",
+              "exchange_id": "plop",
               "timestamp": 1502962946216,
               "datetime": "2017-08-17 12:42:48.000",
               "symbol": "ETH/BTC",
               "order": "12345-67890:09876/54321",
               "type": "limit",
               "side": "buy",
               "takerOrMaker": "taker",
@@ -82,14 +83,15 @@
             }
             """)
 
         trade = create_trade_instance_from_raw(trader, raw_trade)
 
         assert trade.trade_id == '12345-67890:09876/54321'
         assert trade.origin_order_id == '12345-67890:09876/54321'
+        assert trade.exchange_order_id == 'plop'
         assert trade.trade_type == TraderOrderType.BUY_LIMIT
         assert trade.symbol == 'ETH/BTC'
         assert trade.total_cost == decimal.Decimal(str(0.10376526))
         assert trade.executed_quantity == decimal.Decimal(str(1.5))
         assert trade.origin_price == decimal.Decimal(str(0.06917684))
         assert trade.executed_price == decimal.Decimal(str(0.06917684))
         assert trade.executed_time == 1502962946216
@@ -109,14 +111,15 @@
         _, exchange_manager, trader = await self.init_default()
 
         # limit order
         raw_order = json.loads(
             """
             {
                 "id":                "12345-67890:09876/54321",
+                "exchange_id":       "12345-67890:09876/1111",
                 "datetime":          "2017-08-17 12:42:48.000",
                 "timestamp":          1502962946216,
                 "lastTradeTimestamp": 1502962956216,
                 "status":     "open",
                 "symbol":     "BTC/USDT",
                 "type":       "limit",
                 "side":       "sell",
@@ -137,14 +140,15 @@
 
         order = create_order_instance_from_raw(trader, raw_order)
         order.tag = "tag"
         trade = create_trade_from_order(order, close_status=OrderStatus.FILLED)
 
         assert trade.trade_id == '12345-67890:09876/54321'
         assert trade.origin_order_id == '12345-67890:09876/54321'
+        assert trade.exchange_order_id == '12345-67890:09876/1111'
         assert trade.simulated is True
         assert trade.trade_type == TraderOrderType.SELL_LIMIT
         assert trade.symbol == 'BTC/USDT'
         assert trade.total_cost == decimal.Decimal(str(0.076094524))
         assert trade.executed_quantity == decimal.Decimal(str(1.1))
         assert trade.origin_quantity == decimal.Decimal(str(1.5))
         assert trade.origin_price == decimal.Decimal("7684")
@@ -159,14 +163,15 @@
         exec_time = time.time()
         trade = create_trade_from_order(order, executed_time=exec_time)
         assert trade.executed_time == exec_time
 
         # market order
         raw_order = {
             'id': '362550114',
+            'exchange_id': 'AaaaAA',
             'clientOrderId': 'x-T9698eeeeeeeeeeeeee792',
             'timestamp': 1637579281.377,
             'datetime': '2021-11-22T11:08:01.377Z',
             'lastTradeTimestamp': None,
             'symbol': 'UNI/USDT',
             'type': 'market',
             'timeInForce': 'GTC',
@@ -185,14 +190,15 @@
             'fees': []
         }
         order = create_order_instance_from_raw(trader, raw_order)
         trade = create_trade_from_order(order, close_status=OrderStatus.FILLED)
 
         assert trade.trade_id == '362550114'
         assert trade.origin_order_id == '362550114'
+        assert trade.exchange_order_id == 'AaaaAA'
         assert trade.trade_type == TraderOrderType.SELL_MARKET
         assert trade.symbol == 'UNI/USDT'
         assert trade.total_cost == ZERO
         assert trade.executed_quantity == decimal.Decimal("44964.0")
         assert trade.origin_quantity == decimal.Decimal("44964.0")
         assert trade.origin_price == ZERO
         assert trade.executed_price == ZERO
@@ -204,15 +210,15 @@
 
     async def test_create_trade_from_partially_filled_order(self):
         _, exchange_manager, trader = await self.init_default()
 
         raw_order = json.loads(
             """
             {
-                "id":                "12345-67890:09876/54321",
+                "exchange_id":       "plopplip",
                 "datetime":          "2017-08-17 12:42:48.000",
                 "timestamp":          1502962946216,
                 "lastTradeTimestamp": 1502962956216,
                 "status":     "open",
                 "symbol":     "BTC/USDT",
                 "type":       "limit",
                 "side":       "sell",
@@ -230,16 +236,17 @@
                 "info": {}
             }
             """)
 
         order = create_order_instance_from_raw(trader, raw_order)
         trade = create_trade_from_order(order, close_status=OrderStatus.OPEN)
 
-        assert trade.trade_id == '12345-67890:09876/54321'
-        assert trade.origin_order_id == '12345-67890:09876/54321'
+        assert trade.trade_id is not None
+        assert trade.origin_order_id == trade.trade_id
+        assert trade.exchange_order_id == 'plopplip'
         assert trade.simulated is True
         assert trade.trade_type == TraderOrderType.SELL_LIMIT
         assert trade.symbol == 'BTC/USDT'
         assert trade.total_cost == decimal.Decimal(str(0.076094524))
         assert trade.executed_quantity == decimal.Decimal(str(1.1))
         assert trade.origin_quantity == decimal.Decimal(str(1.5))
         assert trade.origin_price == decimal.Decimal(str(7684))
```

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/trades/test_trade_manager.py` & `OctoBot-Trading-2.4.3/tests/personal_data/trades/test_trade_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,46 +25,47 @@
 
 @pytest.fixture
 def trade_manager_and_trader(simulated_trader):
     _, _, trader_instance = simulated_trader
     return personal_data.TradesManager(trader_instance), trader_instance
 
 
-def test_has_closing_trade_with_order_id(trade_manager_and_trader):
+def test_has_closing_trade_with_exchange_order_id(trade_manager_and_trader):
     trade_manager, trader = trade_manager_and_trader
-    assert trade_manager.has_closing_trade_with_order_id(None) is False
-    assert trade_manager.has_closing_trade_with_order_id("None") is False
+    assert trade_manager.has_closing_trade_with_exchange_order_id(None) is False
+    assert trade_manager.has_closing_trade_with_exchange_order_id("None") is False
     trade = create_trade(trader, "id", False, "None")
+    trade.exchange_order_id = "plop"
     trade_manager.trades["id"] = trade
     # trade is not closing order not has the right origin_order_id
-    assert trade_manager.has_closing_trade_with_order_id("id") is False
-    # trade does not has the right origin_order_id
+    assert trade_manager.has_closing_trade_with_exchange_order_id("id") is False
+    # trade does not have the right exchange_order_id
     trade.is_closing_order = True
-    assert trade_manager.has_closing_trade_with_order_id("id2") is False
-    assert trade_manager.has_closing_trade_with_order_id("id") is False
-    trade.origin_order_id = "id"
+    assert trade_manager.has_closing_trade_with_exchange_order_id("id2") is False
+    assert trade_manager.has_closing_trade_with_exchange_order_id("id") is False
+    trade.exchange_order_id = "id"
     # trade is closing this order
-    assert trade_manager.has_closing_trade_with_order_id("id") is True
+    assert trade_manager.has_closing_trade_with_exchange_order_id("id") is True
 
 
 def test_get_completed_trades_pnl(trade_manager_and_trader):
     trade_manager, trader = trade_manager_and_trader
     # no trades
     assert trade_manager.get_completed_trades_pnl() == []
     # with trades
-    for trade_id in (str(i) for i in range(1, 21)):
-        trade_manager.trades[trade_id] = create_trade(
+    for trade_order_id in (str(i) for i in range(1, 21)):
+        trade_manager.trades[trade_order_id] = create_trade(
             trader,
-            trade_id,
+            trade_order_id,
             False,
-            trade_id,
+            trade_order_id,
         )
     # associate first 5 together
-    for trade_id in range(1, 6):
-        trade_manager.get_trade(str(trade_id)).associated_entry_ids = [str(trade_id + 1)]
+    for trade_order_id in range(1, 6):
+        trade_manager.get_trade(str(trade_order_id)).associated_entry_ids = [str(trade_order_id + 1)]
     assert len(trade_manager.get_completed_trades_pnl()) == 5
     trade_manager.get_trade("2").associated_entry_ids.append("10")
     assert len(trade_manager.get_completed_trades_pnl()) == 6
     trade_manager.get_trade("6").associated_entry_ids = ["10"]
     assert len(trade_manager.get_completed_trades_pnl()) == 6
     trade_manager.get_trade("4").status = enums.OrderStatus.CANCELED    # will not be counted
```

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/trades/test_trade_pnl.py` & `OctoBot-Trading-2.4.3/tests/personal_data/trades/test_trade_pnl.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/transactions/__init__.py` & `OctoBot-Trading-2.4.3/tests/personal_data/transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/transactions/test_transaction_factory.py` & `OctoBot-Trading-2.4.3/tests/personal_data/transactions/test_transaction_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/personal_data/transactions/test_transactions_manager.py` & `OctoBot-Trading-2.4.3/tests/personal_data/transactions/test_transactions_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/signals/__init__.py` & `OctoBot-Trading-2.4.3/tests/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/signals/test_trading_signal_bundle_builder.py` & `OctoBot-Trading-2.4.3/tests/signals/test_trading_signal_bundle_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 def test_add_created_order(trading_signal_bundle_builder, buy_limit_order):
     with pytest.raises(errors.InvalidArgumentError):
         trading_signal_bundle_builder.add_created_order(buy_limit_order, buy_limit_order.exchange_manager)
     trading_signal_bundle_builder.add_created_order(buy_limit_order, buy_limit_order.exchange_manager, target_amount="1%")
     assert len(trading_signal_bundle_builder.signals) == 1
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalCommonsAttrs.ACTION.value] \
            is enums.TradingSignalOrdersActions.CREATE.value
-    assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.SHARED_SIGNAL_ORDER_ID.value] == \
-           buy_limit_order.shared_signal_order_id
+    assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.ORDER_ID.value] == \
+           buy_limit_order.order_id
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.TYPE.value] == enums.TraderOrderType.BUY_LIMIT.value
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.TARGET_AMOUNT.value] == "1%"
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.TARGET_POSITION.value] is None
 
     # add the same order: do not add it twice
     trading_signal_bundle_builder.add_created_order(buy_limit_order, buy_limit_order.exchange_manager, target_amount="1%")
     assert len(trading_signal_bundle_builder.signals) == 1
@@ -70,41 +70,41 @@
     buy_limit_order.order_type = enums.TraderOrderType.SELL_LIMIT
     trading_signal_bundle_builder.add_created_order(buy_limit_order, buy_limit_order.exchange_manager, target_position="2%")
     assert len(trading_signal_bundle_builder.signals) == 1
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.TYPE.value] == enums.TraderOrderType.SELL_LIMIT.value
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.TARGET_AMOUNT.value] is None
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.TARGET_POSITION.value] == "2%"
 
-    # add new order (orders are based on shared_signal_order_id)
-    previous_shared_signal_order_id= buy_limit_order.shared_signal_order_id
-    buy_limit_order.set_shared_signal_order_id("other_id")
+    # add new order (orders are based on order_id)
+    previous_order_id = buy_limit_order.order_id
+    buy_limit_order.order_id = "other_id"
     buy_limit_order.order_type = enums.TraderOrderType.STOP_LOSS_LIMIT
     trading_signal_bundle_builder.add_created_order(buy_limit_order, buy_limit_order.exchange_manager, target_position="50")
     assert len(trading_signal_bundle_builder.signals) == 2
-    assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.SHARED_SIGNAL_ORDER_ID.value] == \
-           previous_shared_signal_order_id
+    assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.ORDER_ID.value] == \
+           previous_order_id
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.TYPE.value] == enums.TraderOrderType.SELL_LIMIT.value
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.TARGET_AMOUNT.value] is None
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.TARGET_POSITION.value] == "2%"
-    assert trading_signal_bundle_builder.signals[1].content[enums.TradingSignalOrdersAttrs.SHARED_SIGNAL_ORDER_ID.value] == "other_id"
+    assert trading_signal_bundle_builder.signals[1].content[enums.TradingSignalOrdersAttrs.ORDER_ID.value] == "other_id"
     assert trading_signal_bundle_builder.signals[1].content[enums.TradingSignalOrdersAttrs.TYPE.value] == \
            enums.TraderOrderType.STOP_LOSS_LIMIT.value
     assert trading_signal_bundle_builder.signals[1].content[enums.TradingSignalOrdersAttrs.TARGET_AMOUNT.value] is None
     assert trading_signal_bundle_builder.signals[1].content[enums.TradingSignalOrdersAttrs.TARGET_POSITION.value] == "50"
 
 
 def test_add_order_to_group(trading_signal_bundle_builder, buy_limit_order):
     # no order_group
     trading_signal_bundle_builder.add_order_to_group(buy_limit_order, buy_limit_order.exchange_manager)
     # ensure properly added
     assert len(trading_signal_bundle_builder.signals) == 1
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalCommonsAttrs.ACTION.value] \
            is enums.TradingSignalOrdersActions.ADD_TO_GROUP.value
-    assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.SHARED_SIGNAL_ORDER_ID.value] == \
-           buy_limit_order.shared_signal_order_id
+    assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.ORDER_ID.value] == \
+           buy_limit_order.order_id
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.TYPE.value] == enums.TraderOrderType.BUY_LIMIT.value
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.TARGET_AMOUNT.value] is None
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.TARGET_POSITION.value] is None
 
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.GROUP_ID.value] is None
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.GROUP_TYPE.value] is None
 
@@ -133,16 +133,16 @@
     buy_limit_order.add_to_order_group(other_order_group)
     trading_signal_bundle_builder.add_order_to_group(buy_limit_order, buy_limit_order.exchange_manager)
     assert len(trading_signal_bundle_builder.signals) == 1
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.GROUP_ID.value] == "group_name_2"
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.GROUP_TYPE.value] == \
            personal_data.BalancedTakeProfitAndStopOrderGroup.__name__
 
-    # add new order (orders are based on shared_signal_order_id)
-    buy_limit_order.set_shared_signal_order_id("other_id")
+    # add new order (orders are based on order_id)
+    buy_limit_order.order_id = "other_id"
     buy_limit_order.add_to_order_group(order_group)
     trading_signal_bundle_builder.add_order_to_group(buy_limit_order, buy_limit_order.exchange_manager)
     assert len(trading_signal_bundle_builder.signals) == 2
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.GROUP_ID.value] == "group_name_2"
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.GROUP_TYPE.value] == \
            personal_data.BalancedTakeProfitAndStopOrderGroup.__name__
     assert trading_signal_bundle_builder.signals[1].content[enums.TradingSignalOrdersAttrs.GROUP_ID.value] == "group_name"
@@ -156,16 +156,16 @@
         trading_signal_bundle_builder.add_edited_order(buy_limit_order, buy_limit_order.exchange_manager)
 
     trading_signal_bundle_builder.add_edited_order(buy_limit_order, buy_limit_order.exchange_manager, updated_target_amount="1%")
     # ensure properly added
     assert len(trading_signal_bundle_builder.signals) == 1
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalCommonsAttrs.ACTION.value] \
            is enums.TradingSignalOrdersActions.EDIT.value
-    assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.SHARED_SIGNAL_ORDER_ID.value] == \
-           buy_limit_order.shared_signal_order_id
+    assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.ORDER_ID.value] == \
+           buy_limit_order.order_id
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.TYPE.value] == enums.TraderOrderType.BUY_LIMIT.value
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.TARGET_AMOUNT.value] == "1%"
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.TARGET_POSITION.value] is None
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.UPDATED_TARGET_AMOUNT.value] == "1%"
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.UPDATED_TARGET_POSITION.value] is None
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.UPDATED_LIMIT_PRICE.value] == 0.0
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.UPDATED_STOP_PRICE.value] == 0.0
@@ -209,53 +209,53 @@
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.TARGET_POSITION.value] is None
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.UPDATED_TARGET_AMOUNT.value] is None
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.UPDATED_TARGET_POSITION.value] is None
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.UPDATED_LIMIT_PRICE.value] == 0.0
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.UPDATED_STOP_PRICE.value] == 0.0
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.UPDATED_CURRENT_PRICE.value] == 1.0
 
-    # add new order (orders are based on shared_signal_order_id)
-    buy_limit_order.set_shared_signal_order_id("other_id")
+    # add new order (orders are based on order_id)
+    buy_limit_order.order_id = "other_id"
     trading_signal_bundle_builder.add_edited_order(buy_limit_order, buy_limit_order.exchange_manager, updated_target_position="1%a")
     assert len(trading_signal_bundle_builder.signals) == 2
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.UPDATED_CURRENT_PRICE.value] == 1.0
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.UPDATED_TARGET_POSITION.value] == None
     assert trading_signal_bundle_builder.signals[1].content[enums.TradingSignalOrdersAttrs.UPDATED_CURRENT_PRICE.value] == 0.0
     assert trading_signal_bundle_builder.signals[1].content[enums.TradingSignalOrdersAttrs.UPDATED_TARGET_POSITION.value] == "1%a"
 
 
 @pytest.mark.asyncio
 async def test_add_cancelled_order(trading_signal_bundle_builder, buy_limit_order):
     trading_signal_bundle_builder.add_cancelled_order(buy_limit_order, buy_limit_order.exchange_manager)
     assert len(trading_signal_bundle_builder.signals) == 1
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalCommonsAttrs.ACTION.value] \
            is enums.TradingSignalOrdersActions.CANCEL.value
-    assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.SHARED_SIGNAL_ORDER_ID.value] == \
-           buy_limit_order.shared_signal_order_id
+    assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.ORDER_ID.value] == \
+           buy_limit_order.order_id
 
     # add the same order: do not add it twice
     trading_signal_bundle_builder.add_cancelled_order(buy_limit_order, buy_limit_order.exchange_manager)
     assert len(trading_signal_bundle_builder.signals) == 1
 
-    # add new order (orders are based on shared_signal_order_id)
+    # add new order (orders are based on order_id)
     # cancel order first to be sure it can be added
     exchange_manager = buy_limit_order.exchange_manager
     await buy_limit_order.exchange_manager.trader.cancel_order(buy_limit_order)
     buy_limit_order.clear()
-    buy_limit_order.set_shared_signal_order_id("other_id")
+    buy_limit_order.order_id = "other_id"
     buy_limit_order.order_type = enums.TraderOrderType.STOP_LOSS_LIMIT
     trading_signal_bundle_builder.add_created_order(buy_limit_order, exchange_manager, target_position="50")
     assert len(trading_signal_bundle_builder.signals) == 2
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.TYPE.value] == enums.TraderOrderType.BUY_LIMIT.value
     assert trading_signal_bundle_builder.signals[1].content[enums.TradingSignalOrdersAttrs.TYPE.value] == \
            enums.TraderOrderType.STOP_LOSS_LIMIT.value
 
     # add an orders via create action: it gets popped out of the orders list as there is no point creating
     # it and cancelling it right away
-    buy_limit_order.set_shared_signal_order_id("buy_other_id")
+    buy_limit_order.order_id = "buy_other_id"
     buy_limit_order.order_type = enums.TraderOrderType.BUY_MARKET
     trading_signal_bundle_builder.add_created_order(buy_limit_order, exchange_manager, target_amount="1")
     assert len(trading_signal_bundle_builder.signals) == 3
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.TYPE.value] == enums.TraderOrderType.BUY_LIMIT.value
     assert trading_signal_bundle_builder.signals[1].content[enums.TradingSignalOrdersAttrs.TYPE.value] == \
            enums.TraderOrderType.STOP_LOSS_LIMIT.value
     assert trading_signal_bundle_builder.signals[2].content[enums.TradingSignalOrdersAttrs.TYPE.value] == enums.TraderOrderType.BUY_MARKET.value
@@ -289,15 +289,15 @@
     assert trading_signal_bundle_builder.signals[1].content[enums.TradingSignalOrdersAttrs.TYPE.value] == \
            enums.TraderOrderType.STOP_LOSS_LIMIT.value
     assert trading_signal_bundle_builder.signals[2].content[enums.TradingSignalOrdersAttrs.TYPE.value] == enums.TraderOrderType.BUY_MARKET.value
     assert trading_signal_bundle_builder.signals[2].content[enums.TradingSignalCommonsAttrs.ACTION.value] == \
            enums.TradingSignalOrdersActions.CANCEL.value
 
     # adding BUY_MARKET as edited order
-    buy_limit_order.set_shared_signal_order_id("edit_buy_other_id")
+    buy_limit_order.order_id = "edit_buy_other_id"
     trading_signal_bundle_builder.add_edited_order(buy_limit_order, exchange_manager, updated_target_amount="1")
     assert len(trading_signal_bundle_builder.signals) == 4
     assert trading_signal_bundle_builder.signals[0].content[enums.TradingSignalOrdersAttrs.TYPE.value] == enums.TraderOrderType.BUY_LIMIT.value
     assert trading_signal_bundle_builder.signals[1].content[enums.TradingSignalOrdersAttrs.TYPE.value] == \
            enums.TraderOrderType.STOP_LOSS_LIMIT.value
     assert trading_signal_bundle_builder.signals[2].content[enums.TradingSignalOrdersAttrs.TYPE.value] == enums.TraderOrderType.BUY_MARKET.value
     assert trading_signal_bundle_builder.signals[2].content[enums.TradingSignalCommonsAttrs.ACTION.value] == \
@@ -318,17 +318,17 @@
     assert trading_signal_bundle_builder.signals[3].content[enums.TradingSignalOrdersAttrs.TYPE.value] == enums.TraderOrderType.BUY_MARKET.value
     assert trading_signal_bundle_builder.signals[3].content[enums.TradingSignalCommonsAttrs.ACTION.value] == \
            enums.TradingSignalOrdersActions.CANCEL.value
 
 
 def test_pack_referenced_orders_together(trading_signal_bundle_builder,
                                          buy_limit_order, sell_limit_order, stop_loss_limit_order, stop_loss_buy_order):
-    buy_limit_order.set_shared_signal_order_id("0")
-    sell_limit_order.set_shared_signal_order_id("1")
-    stop_loss_limit_order.set_shared_signal_order_id("2")
+    buy_limit_order.order_id = "0"
+    sell_limit_order.order_id = "1"
+    stop_loss_limit_order.order_id = "2"
     trading_signal_bundle_builder.add_created_order(buy_limit_order, buy_limit_order.exchange_manager, target_amount="1%")
     trading_signal_bundle_builder.add_created_order(sell_limit_order, buy_limit_order.exchange_manager, target_amount="1%")
     trading_signal_bundle_builder.add_created_order(stop_loss_limit_order, buy_limit_order.exchange_manager, target_amount="1%")
     assert len(trading_signal_bundle_builder.signals) == 3
     assert all(signal.content[enums.TradingSignalOrdersAttrs.ADDITIONAL_ORDERS.value] == []
                for signal in trading_signal_bundle_builder.signals)
     pre_pack_signals = copy.copy(trading_signal_bundle_builder.signals)
```

### Comparing `OctoBot-Trading-2.4.2/tests/signals/test_util.py` & `OctoBot-Trading-2.4.3/tests/signals/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         enums.TradingSignalOrdersAttrs.CURRENT_PRICE.value: float(buy_limit_order.created_last_price),
         enums.TradingSignalOrdersAttrs.UPDATED_CURRENT_PRICE.value: 0.0,
         enums.TradingSignalOrdersAttrs.REDUCE_ONLY.value: True,
         enums.TradingSignalOrdersAttrs.POST_ONLY.value: False,
         enums.TradingSignalOrdersAttrs.GROUP_ID.value: None,
         enums.TradingSignalOrdersAttrs.GROUP_TYPE.value: None,
         enums.TradingSignalOrdersAttrs.TAG.value: "hello",
-        enums.TradingSignalOrdersAttrs.SHARED_SIGNAL_ORDER_ID.value: buy_limit_order.shared_signal_order_id,
+        enums.TradingSignalOrdersAttrs.ORDER_ID.value: buy_limit_order.order_id,
         enums.TradingSignalOrdersAttrs.BUNDLED_WITH.value: None,
         enums.TradingSignalOrdersAttrs.CHAINED_TO.value: None,
         enums.TradingSignalOrdersAttrs.ADDITIONAL_ORDERS.value: [],
         enums.TradingSignalOrdersAttrs.ASSOCIATED_ORDER_IDS.value: None,
     }
 
     sell_limit_order.add_chained_order(buy_limit_order)
@@ -98,17 +98,17 @@
         enums.TradingSignalOrdersAttrs.CURRENT_PRICE.value: float(buy_limit_order.created_last_price),
         enums.TradingSignalOrdersAttrs.UPDATED_CURRENT_PRICE.value: 0.0,
         enums.TradingSignalOrdersAttrs.REDUCE_ONLY.value: True,
         enums.TradingSignalOrdersAttrs.POST_ONLY.value: False,
         enums.TradingSignalOrdersAttrs.GROUP_ID.value: None,
         enums.TradingSignalOrdersAttrs.GROUP_TYPE.value: None,
         enums.TradingSignalOrdersAttrs.TAG.value: "hello",
-        enums.TradingSignalOrdersAttrs.SHARED_SIGNAL_ORDER_ID.value: buy_limit_order.shared_signal_order_id,
-        enums.TradingSignalOrdersAttrs.BUNDLED_WITH.value: sell_limit_order.shared_signal_order_id,
-        enums.TradingSignalOrdersAttrs.CHAINED_TO.value: sell_limit_order.shared_signal_order_id,
+        enums.TradingSignalOrdersAttrs.ORDER_ID.value: buy_limit_order.order_id,
+        enums.TradingSignalOrdersAttrs.BUNDLED_WITH.value: sell_limit_order.order_id,
+        enums.TradingSignalOrdersAttrs.CHAINED_TO.value: sell_limit_order.order_id,
         enums.TradingSignalOrdersAttrs.ADDITIONAL_ORDERS.value: [],
         enums.TradingSignalOrdersAttrs.ASSOCIATED_ORDER_IDS.value: ["1"],
     }
 
     order_group = personal_data.OneCancelsTheOtherOrderGroup(
         "group_name",
         buy_limit_order.exchange_manager.exchange_personal_data.orders_manager
@@ -136,17 +136,17 @@
         enums.TradingSignalOrdersAttrs.CURRENT_PRICE.value: 111.0,
         enums.TradingSignalOrdersAttrs.UPDATED_CURRENT_PRICE.value: 111.0,
         enums.TradingSignalOrdersAttrs.REDUCE_ONLY.value: True,
         enums.TradingSignalOrdersAttrs.POST_ONLY.value: False,
         enums.TradingSignalOrdersAttrs.GROUP_ID.value: order_group.name,
         enums.TradingSignalOrdersAttrs.GROUP_TYPE.value: personal_data.OneCancelsTheOtherOrderGroup.__name__,
         enums.TradingSignalOrdersAttrs.TAG.value: "hello",
-        enums.TradingSignalOrdersAttrs.SHARED_SIGNAL_ORDER_ID.value: buy_limit_order.shared_signal_order_id,
-        enums.TradingSignalOrdersAttrs.BUNDLED_WITH.value: sell_limit_order.shared_signal_order_id,
-        enums.TradingSignalOrdersAttrs.CHAINED_TO.value: sell_limit_order.shared_signal_order_id,
+        enums.TradingSignalOrdersAttrs.ORDER_ID.value: buy_limit_order.order_id,
+        enums.TradingSignalOrdersAttrs.BUNDLED_WITH.value: sell_limit_order.order_id,
+        enums.TradingSignalOrdersAttrs.CHAINED_TO.value: sell_limit_order.order_id,
         enums.TradingSignalOrdersAttrs.ADDITIONAL_ORDERS.value: [],
         enums.TradingSignalOrdersAttrs.ASSOCIATED_ORDER_IDS.value: ["1", "2", "3"],
     }
     assert signals.create_order_signal_content(
         buy_limit_order,
         enums.TradingSignalOrdersActions.CREATE,
         "strat",
```

### Comparing `OctoBot-Trading-2.4.2/tests/test_utils/order_util.py` & `OctoBot-Trading-2.4.3/tests/test_utils/order_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/test_utils/random_numbers.py` & `OctoBot-Trading-2.4.3/tests/test_utils/random_numbers.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/util/__init__.py` & `OctoBot-Trading-2.4.3/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests/util/test_config_util.py` & `OctoBot-Trading-2.4.3/tests/util/test_config_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/__init__.py` & `OctoBot-Trading-2.4.3/tests_additional/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/__init__.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/real_exchange_tester.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/real_exchange_tester.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/real_futures_exchange_tester.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/real_futures_exchange_tester.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_ascendex.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_ascendex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_binance.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_binance.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_bitfinex.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_bitfinex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_bitget.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_bitget.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_bithumb.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_bithumb.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_bitso.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_bitso.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_bitstamp.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_bitstamp.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_bittrex.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_bittrex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_bybit.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_bybit.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_bybit_futures.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_bybit_futures.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_coinbase.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_coinbase.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_coinex.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_coinex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_cryptocom.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_cryptocom.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_gateio.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_gateio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_hitbtc.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_hitbtc.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_hollaex.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_hollaex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_huobi.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_huobi.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_huobipro.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_huobipro.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_kraken.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_kraken.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_kucoin.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_kucoin.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_kucoin_futures.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_kucoin_futures.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_ndax.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_ndax.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_okcoin.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_okcoin.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_okx.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_okx.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_okx_futures.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_okx_futures.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_phemex.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_phemex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_poloniex.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_poloniex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_upbit.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_upbit.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.2/tests_additional/real_exchanges/test_wavesexchange.py` & `OctoBot-Trading-2.4.3/tests_additional/real_exchanges/test_wavesexchange.py`

 * *Files identical despite different names*

