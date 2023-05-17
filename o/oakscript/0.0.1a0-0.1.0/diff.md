# Comparing `tmp/oakscript-0.0.1a0.tar.gz` & `tmp/oakscript-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oakscript-0.0.1a0.tar", last modified: Wed May 17 06:38:10 2023, max compression
+gzip compressed data, was "oakscript-0.1.0.tar", last modified: Sat May 13 18:02:55 2023, max compression
```

## Comparing `oakscript-0.0.1a0.tar` & `oakscript-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:38:10.398594 oakscript-0.0.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-17 06:38:10.398594 oakscript-0.0.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-17 06:38:00.000000 oakscript-0.0.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:38:10.394594 oakscript-0.0.1a0/oakscript/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:38:00.000000 oakscript-0.0.1a0/oakscript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:38:10.394594 oakscript-0.0.1a0/oakscript/pinescript/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-17 06:38:00.000000 oakscript-0.0.1a0/oakscript/pinescript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-17 06:38:00.000000 oakscript-0.0.1a0/oakscript/pinescript/ta.py
--rw-r--r--   0 runner    (1001) docker     (123)    20419 2023-05-17 06:38:00.000000 oakscript-0.0.1a0/oakscript/screener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:38:10.394594 oakscript-0.0.1a0/oakscript/strategytester/
--rw-r--r--   0 runner    (1001) docker     (123)    21787 2023-05-17 06:38:00.000000 oakscript-0.0.1a0/oakscript/strategytester/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:38:10.394594 oakscript-0.0.1a0/oakscript/strategytester/reports/
--rw-r--r--   0 runner    (1001) docker     (123)    23252 2023-05-17 06:38:00.000000 oakscript-0.0.1a0/oakscript/strategytester/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-17 06:38:00.000000 oakscript-0.0.1a0/oakscript/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:38:10.394594 oakscript-0.0.1a0/oakscript.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-17 06:38:10.000000 oakscript-0.0.1a0/oakscript.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-17 06:38:10.000000 oakscript-0.0.1a0/oakscript.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 06:38:10.000000 oakscript-0.0.1a0/oakscript.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 06:38:10.000000 oakscript-0.0.1a0/oakscript.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 06:38:10.398594 oakscript-0.0.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-17 06:38:00.000000 oakscript-0.0.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:38:10.398594 oakscript-0.0.1a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:38:00.000000 oakscript-0.0.1a0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:38:10.398594 oakscript-0.0.1a0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:38:00.000000 oakscript-0.0.1a0/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:38:10.398594 oakscript-0.0.1a0/tests/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-17 06:38:00.000000 oakscript-0.0.1a0/tests/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-17 06:38:00.000000 oakscript-0.0.1a0/tests/strategies/rsi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 18:02:55.888521 oakscript-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-13 18:02:55.888521 oakscript-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-13 18:02:47.000000 oakscript-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 18:02:55.888521 oakscript-0.1.0/oakscript/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-13 18:02:47.000000 oakscript-0.1.0/oakscript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 18:02:55.888521 oakscript-0.1.0/oakscript/pinescript/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-13 18:02:47.000000 oakscript-0.1.0/oakscript/pinescript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-13 18:02:47.000000 oakscript-0.1.0/oakscript/pinescript/ta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20419 2023-05-13 18:02:47.000000 oakscript-0.1.0/oakscript/screener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 18:02:55.888521 oakscript-0.1.0/oakscript/strategytester/
+-rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-05-13 18:02:47.000000 oakscript-0.1.0/oakscript/strategytester/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 18:02:55.888521 oakscript-0.1.0/oakscript/strategytester/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)    23845 2023-05-13 18:02:47.000000 oakscript-0.1.0/oakscript/strategytester/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 18:02:55.888521 oakscript-0.1.0/oakscript.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-13 18:02:55.000000 oakscript-0.1.0/oakscript.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-13 18:02:55.000000 oakscript-0.1.0/oakscript.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 18:02:55.000000 oakscript-0.1.0/oakscript.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-13 18:02:55.000000 oakscript-0.1.0/oakscript.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-13 18:02:47.000000 oakscript-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 18:02:55.888521 oakscript-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-13 18:02:47.000000 oakscript-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 18:02:55.888521 oakscript-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 18:02:47.000000 oakscript-0.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 18:02:55.888521 oakscript-0.1.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 18:02:47.000000 oakscript-0.1.0/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 18:02:55.888521 oakscript-0.1.0/tests/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-13 18:02:47.000000 oakscript-0.1.0/tests/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-13 18:02:47.000000 oakscript-0.1.0/tests/strategies/rsi.py
```

### Comparing `oakscript-0.0.1a0/oakscript/pinescript/__init__.py` & `oakscript-0.1.0/oakscript/pinescript/__init__.py`

 * *Files identical despite different names*

### Comparing `oakscript-0.0.1a0/oakscript/screener.py` & `oakscript-0.1.0/oakscript/screener.py`

 * *Files identical despite different names*

### Comparing `oakscript-0.0.1a0/oakscript/strategytester/reports/__init__.py` & `oakscript-0.1.0/oakscript/strategytester/reports/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,66 @@
 import math
-from _decimal import ROUND_UP
-from decimal import Decimal, ROUND_HALF_UP, ROUND_DOWN
+from decimal import Decimal, ROUND_HALF_UP
 import numpy as np
 import pandas as pd
 
-from oakscript.util import get_marketdata_range, percent, roundhalfup, safe_div
-
 rename_columns = {'entry_price': 'Price', 'date_time': 'Date/Time',
                   'type': 'Type', 'signal': 'Signal', 'contracts': 'Contracts',
                   'trade_num': 'Trade #', 'profit': 'Profit'
                   }
 filter_columns = ['Trade #', 'Type', 'Signal', 'Date/Time', 'Price', 'Contracts', 'Profit', 'Profit %', 'Cum. Profit',
                   'Cum. Profit %', 'Run-up', 'Run-up %',
                   'Drawdown', 'Drawdown %'
                   ]
 
 
+def percent(start, end):
+    return 100 * (end - start) / start
+
+
+def get_market_data_range(marketdata, entry_date, close_date, entry_price="open", close_price="open"):
+    marketdata_range = marketdata.loc[close_date:entry_date]
+    first_marketdata = marketdata_range.iloc[-1]
+    last_marketdata = marketdata_range.iloc[0]
+
+
 def get_drawdown(marketdata, trade_entry, trade_close):
     # Trade entry price
-    entry_price = roundhalfup(trade_entry['rounded_price'])
-    exit_price = roundhalfup(trade_close['rounded_price']) or entry_price
+    entry_price = roundup(trade_entry['rounded_price'])
+    exit_price = roundup(trade_close['rounded_price']) or entry_price
 
     # Market data range
     entry_date, exit_date = trade_entry['date_time'], trade_close['date_time']
     if pd.isnull(exit_date):
         exit_date = None
     marketdata_range = get_marketdata_range(marketdata, entry_date, exit_date, entry_price, exit_price)
 
     if is_long(trade_entry):
-        low = roundhalfup(marketdata_range['low'].min())
+        low = roundup(marketdata_range['low'].min())
         drawdown = entry_price - low
         drawdown_pct = percent(entry_price, low)
     else:
-        high = roundhalfup(marketdata_range['high'].max())
+        high = roundup(marketdata_range['high'].max())
         drawdown = high - entry_price
         drawdown_pct = percent(entry_price, high)
     return round(drawdown, 2), round(abs(drawdown_pct), 2)
 
 
+def get_marketdata_range(marketdata, entry_date, exit_date, entry_price, exit_price):
+    marketdata_range = marketdata.loc[exit_date:entry_date].copy()
+    entry_bar = marketdata_range.iloc[-1]
+    exit_bar = marketdata_range.iloc[0]
+
+    # Case 1: There is high/low on closing bar for an exit price at open
+    if exit_price == roundup(exit_bar.open):
+        marketdata_range.iloc[0] = [exit_bar.open, exit_bar.open, exit_bar.open, exit_bar.open]
+    # Case 2: Limit order close at limit
+    else:
+        marketdata_range.iloc[0] = [exit_bar.open, exit_price, exit_price, exit_bar.close]
+    return marketdata_range
 
 
 def process_drawdown(d, marketdata):
     d['Drawdown'] = np.nan
     d['Drawdown %'] = np.nan
     for group_name, df_group in d.groupby('trade_num'):
         trade_entry = df_group.iloc[0]
@@ -71,14 +90,16 @@
 
 
 def get_short_runup(equity_on_entry, min_equity, numbers_of_contracts, current_low, entry_price):
     return equity_on_entry - min_equity + numbers_of_contracts * (entry_price - current_low)
 
 
 def get_max_runup(entry, close, marketdata, initial_equity, min_equity, last_cumulated_profit):
+
+
     entry_price = entry['entry_price']
     exit_price = close['entry_price']
     numbers_of_contracts = entry['contracts']
 
     entry_date, exit_date = entry['date_time'], close['date_time']
     if pd.isnull(exit_date):
         exit_date = None
@@ -95,38 +116,34 @@
         low = min(marketdata_range['low'].min(), exit_price)
         runup = get_long_runup(initial_equity, min_equity, numbers_of_contracts, low, entry_price)
         runup_pct = percent(entry_price, low)
 
     return abs(runup), runup_pct
 
 
-def get_runup(entry, exit, marketdata):
-    if not np.isnan(exit['entry_price']):
+def get_runup(entry, close, marketdata):
+    if not np.isnan(close['entry_price']):
         # Trade entry price
-        entry_price = roundhalfup(entry['entry_price'])
-        exit_price = roundhalfup(exit['entry_price'])
+        entry_price = roundup(entry['entry_price'])
+        exit_price = roundup(close['entry_price'])
 
-        entry_date, exit_date = entry['date_time'], exit['date_time']
+        entry_date, exit_date = entry['date_time'], close['date_time']
         if pd.isnull(exit_date):
             exit_date = None
         marketdata_range = get_marketdata_range(marketdata, entry_date, exit_date, entry_price, exit_price)
 
         if is_short(entry):
-            low = min(roundhalfup(marketdata_range['low'].min()), exit_price)
+            low = min(roundup(marketdata_range['low'].min()), exit_price)
             runup = entry_price - low
             runup_pct = percent(entry_price, low)
         else:
-            high = max(roundhalfup(marketdata_range['high'].max()), exit_price)
-            open_price = marketdata_range.iloc[-1].open  # Get the price not rounded
-            if entry_price == roundhalfup(open_price):
-                runup = high - round(open_price, 2)
-            else:
-                runup = high - entry_price
+            high = max(roundup(marketdata_range['high'].max()), exit_price)
+            runup = high - entry_price
             runup_pct = percent(entry_price, high)
-        return max(runup, 0), runup_pct
+        return runup, runup_pct
     else:
         return None, None
 
 
 def process_max_runup(d, marketdata, initial_equity):
     min_equity = initial_equity
     max_run_up = 0
@@ -169,16 +186,16 @@
     d['Cum. Profit %'] = d.groupby('trade_num', sort=False)['Cum. Profit %'].apply(
         lambda x: x.ffill().bfill())
     return d['Cum. Profit %']
 
 
 def get_profit_pct(entry, close):
     if not np.isnan(entry['entry_price']):
-        entry_price = roundhalfup(entry['entry_price'])
-        close_price = roundhalfup(close['entry_price'])
+        entry_price = roundup(entry['entry_price'])
+        close_price = roundup(close['entry_price'])
 
         if is_short(entry):
             profit_pct = -percent(entry_price, close_price)
         else:
             profit_pct = percent(entry_price, close_price)
         return round(profit_pct, 2)
     else:
@@ -197,25 +214,29 @@
     d["Cum. Profit"] = d[d['type'].str.startswith('Exit')]['profit'].cumsum()
     d['Cum. Profit'] = d.groupby('trade_num', sort=False)['Cum. Profit'].apply(
         lambda x: x.ffill().bfill())
     return d['Cum. Profit']
 
 
 def process_profit(d):
-    d['rounded_price'] = d['entry_price'].apply(lambda x: roundhalfup(x))
+    d['rounded_price'] = d['entry_price'].apply(lambda x: roundup(x))
     d['shift'] = d.groupby('trade_num')['rounded_price'].shift()
     d['profit'] = np.where(d['type'].str.contains('Long'),
                            d['rounded_price'] - d['shift'],
                            d['shift'] - d['rounded_price'])
 
     # Copy the profit value to both rows
     d['profit'] = d.groupby('trade_num')['profit'].apply(lambda x: x.ffill().bfill())
     return d['profit']
 
 
+def roundup(x):
+    return np.nan if math.isinf(x) else float(Decimal(str(x)).quantize(Decimal('.01'), rounding=ROUND_HALF_UP))
+
+
 def process_trades_list(positions, data, initial_capital):
     df_trades = pd.DataFrame([o.__dict__ for o in positions])
     # df_trades['entry_price'] = round(df_trades['entry_price'], 2)
 
     # df_trades['date_time'] = df_trades['date_time'].dt.date
     # df_trades[['profit', 'Cum. Profit', 'Run-up', 'Drawdown']] = None
     # TODO move code prior to rename column
@@ -223,18 +244,18 @@
     df_trades['Cum. Profit'] = process_cumulative_profit(df_trades)
     df_trades['Profit %'] = process_profit_pct(df_trades)
     # TODO Get the initial equity for cum profit pct
     df_trades['Cum. Profit %'] = process_cumulative_profit_pct(df_trades)
     df_trades['Run-up'], df_trades['Run-up %'] = process_runup(df_trades, data, initial_capital)
     df_trades['Drawdown'], df_trades['Drawdown %'] = process_drawdown(df_trades, data)
 
-    df_trades['entry_price'] = df_trades['entry_price'].map(lambda x: roundhalfup(x))
+    df_trades['entry_price'] = df_trades['entry_price'].map(lambda x: roundup(x))
     # df_trades['profit'] = df_trades['profit'].map(
     #    lambda x: roundup(x))
-    df_trades['Cum. Profit'] = df_trades['Cum. Profit'].map(lambda x: roundhalfup(x))
+    df_trades['Cum. Profit'] = df_trades['Cum. Profit'].map(lambda x: roundup(x))
 
     df_trades['contracts'] = df_trades['contracts'].map(lambda x: abs(x) if x != 0 else np.nan)
     # df_trades.iloc[-1]['contracts'] = np.nan
     return df_trades  # .rename(columns=rename_columns)[filter_columns]
 
 
 def get_sharpe_ratio(return_series, N, rf):
@@ -254,97 +275,101 @@
     highest_price = marketdata.loc[:entry_date]['high'].max()
 
     if 'Long' in last_trade_entry['type']:
         dd = lowest_price - entry_price
     else:
         dd = entry_price - highest_price
     profits = trades_list[trades_list['type'].str.startswith('Entry')]['profit'].values
-    dd = roundhalfup(dd)
+    dd = roundup(dd)
     profits = np.append(profits, dd)
     profits = profits[~np.isnan(profits)]
     cs = np.cumsum(profits)
     max_dd = np.max(cs) - np.min(cs)
     return max_dd
 
 
+def safe_div(n, d):
+    return n / d if d else 0
+
+
 def process_performance_summary(trades_list, market_positions, marketdata, initial_capital):
     cols = ["Title", "All", "All %", "Long", "Long %", "Short", "Short %"]
     df_perf = pd.DataFrame(columns=cols)
     performance_summary = [cols]
 
-    net_profit = roundhalfup(trades_list['profit'].sum() / 2)
-    net_profit_perc = roundhalfup(percent(initial_capital, initial_capital + net_profit))
-    net_profit_long = roundhalfup(trades_list[trades_list['type'].str.contains('Long')]['profit'].sum() / 2)
-    net_profit_long_perc = roundhalfup(percent(initial_capital, initial_capital + net_profit_long))
-    net_profit_short = roundhalfup(trades_list[trades_list['type'].str.contains('Short')]['profit'].sum() / 2)
-    net_profit_short_perc = roundhalfup(percent(initial_capital, initial_capital + net_profit_short))
+    net_profit = roundup(trades_list['profit'].sum() / 2)
+    net_profit_perc = roundup(percent(initial_capital, initial_capital + net_profit))
+    net_profit_long = roundup(trades_list[trades_list['type'].str.contains('Long')]['profit'].sum() / 2)
+    net_profit_long_perc = roundup(percent(initial_capital, initial_capital + net_profit_long))
+    net_profit_short = roundup(trades_list[trades_list['type'].str.contains('Short')]['profit'].sum() / 2)
+    net_profit_short_perc = roundup(percent(initial_capital, initial_capital + net_profit_short))
     net_profit_series = pd.Series(
         ["Net Profit", net_profit, net_profit_perc, net_profit_long, net_profit_long_perc, net_profit_short,
          net_profit_short_perc],
         index=cols)
     df_perf = pd.concat([df_perf, net_profit_series.to_frame().T], ignore_index=True)
 
-    gross_profit = roundhalfup(trades_list[trades_list['profit'] > 0]['profit'].sum() / 2)
-    gross_profit_perc = roundhalfup(percent(initial_capital, initial_capital + gross_profit))
-    gross_profit_long = roundhalfup(
+    gross_profit = roundup(trades_list[trades_list['profit'] > 0]['profit'].sum() / 2)
+    gross_profit_perc = roundup(percent(initial_capital, initial_capital + gross_profit))
+    gross_profit_long = roundup(
         trades_list[(trades_list['profit'] > 0) & (trades_list['type'].str.contains('Long'))]['profit'].sum() / 2)
-    gross_profit_long_perc = roundhalfup(percent(initial_capital, initial_capital + gross_profit_long))
-    gross_profit_short = roundhalfup(
+    gross_profit_long_perc = roundup(percent(initial_capital, initial_capital + gross_profit_long))
+    gross_profit_short = roundup(
         trades_list[(trades_list['profit'] > 0) & (trades_list['type'].str.contains('Short'))]['profit'].sum() / 2)
-    gross_profit_short_perc = roundhalfup(percent(initial_capital, initial_capital + gross_profit_short))
+    gross_profit_short_perc = roundup(percent(initial_capital, initial_capital + gross_profit_short))
     gross_profit_series = pd.Series(
         ["Gross Profit", gross_profit, gross_profit_perc, gross_profit_long, gross_profit_long_perc, gross_profit_short,
          gross_profit_short_perc], index=cols)
     df_perf = pd.concat([df_perf, gross_profit_series.to_frame().T], ignore_index=True)
 
-    gross_loss = abs(roundhalfup(trades_list[trades_list['profit'] < 0]['profit'].sum() / 2))
-    gross_loss_perc = roundhalfup(percent(initial_capital, initial_capital + gross_loss))
-    gross_loss_long = abs(roundhalfup(
+    gross_loss = abs(roundup(trades_list[trades_list['profit'] < 0]['profit'].sum() / 2))
+    gross_loss_perc = roundup(percent(initial_capital, initial_capital + gross_loss))
+    gross_loss_long = abs(roundup(
         trades_list[(trades_list['profit'] < 0) & (trades_list['type'].str.contains('Long'))]['profit'].sum() / 2))
-    gross_loss_long_perc = roundhalfup(percent(initial_capital, initial_capital + gross_loss_long))
-    gross_loss_short = abs(roundhalfup(
+    gross_loss_long_perc = roundup(percent(initial_capital, initial_capital + gross_loss_long))
+    gross_loss_short = abs(roundup(
         trades_list[(trades_list['profit'] < 0) & (trades_list['type'].str.contains('Short'))]['profit'].sum() / 2))
-    gross_loss_short_perc = roundhalfup(percent(initial_capital, initial_capital + gross_loss_short))
+    gross_loss_short_perc = roundup(percent(initial_capital, initial_capital + gross_loss_short))
     gross_loss_series = pd.Series(
         ["Gross Loss", gross_loss, gross_loss_perc, gross_loss_long, gross_loss_long_perc, gross_loss_short,
          gross_loss_short_perc],
         index=cols)
     df_perf = pd.concat([df_perf, gross_loss_series.to_frame().T], ignore_index=True)
 
     max_runup = process_max_runup(trades_list, marketdata, initial_capital)  # trades_list['Run-up'].max()
-    max_runup_perc = roundhalfup(percent(initial_capital, initial_capital + max_runup))
+    max_runup_perc = roundup(percent(initial_capital, initial_capital + max_runup))
     df_perf = pd.concat([df_perf, pd.Series(["Max Run-up", max_runup, max_runup_perc], index=cols[:3]).to_frame().T])
 
     max_drawdown = get_max_drawdown(marketdata, trades_list)
-    max_drawdown_perc = roundhalfup(percent(initial_capital, initial_capital + max_drawdown))
+    max_drawdown_perc = roundup(percent(initial_capital, initial_capital + max_drawdown))
     df_perf = pd.concat(
         [df_perf, pd.Series(["Max Drawdown", max_drawdown, max_drawdown_perc], index=cols[:3]).to_frame().T],
         ignore_index=True)
 
     # Buy & Hold
     first_trade_price = trades_list.iloc[0]['entry_price']
     last_price = marketdata.iloc[0].close
     buy_shares = int(initial_capital / first_trade_price)
     buy_and_hold = buy_shares * last_price - initial_capital
-    buy_and_hold_perc = roundhalfup(buy_and_hold / initial_capital * 100)
+    buy_and_hold_perc = roundup(buy_and_hold / initial_capital * 100)
     df_perf = pd.concat([df_perf, pd.Series(
         ["Buy & Hold Return", buy_and_hold, buy_and_hold_perc], index=cols[:3]).to_frame().T], ignore_index=True)
 
     # Sharpe Ratio
     """The formula for the Sharpe ratio is SR = (MR - RFR) / SD, where MR is the average return for a period (monthly 
     for a trading period of 3 or more months or daily for a trading period of 3 or more days), and RFR is the 
     risk-free rate of return (by default, 2% annually. Can be changed with the "risk_free_rate" parameter of the 
     "strategy()" function). SD is the standard deviation of returns."""
 
     risk_free_rate = 2
     monthly_adj = (21 ** 0.5)
 
     N = 21  # 21 trading days per month
     rf = 0.02  # 2% risk-free rate
-    sharpe_ratio = roundhalfup(get_sharpe_ratio(trades_list['profit'], N, rf, ) * 100)
+    sharpe_ratio = roundup(get_sharpe_ratio(trades_list['profit'], N, rf, ) * 100)
 
     df_perf = pd.concat([df_perf, pd.Series(
         ["Sharpe Ratio", sharpe_ratio], index=cols[:2]).to_frame().T], ignore_index=True)
 
     # Sortino Ratio
     """The formula for the Sortino ratio is SR = (MR - RFR) / DD, where MR is the average return for a period (
     monthly for a trading period of 3 or more months or daily for a trading period of 3 or more days), and RFR is the 
@@ -353,15 +378,15 @@
     return, N - total number of returns, T - target return."""
 
     def get_sortino_ratio(series, N, rf):
         mean = series.mean() * N - rf
         std_neg = series[series < 0].std() * np.sqrt(N)
         return mean / std_neg
 
-    sortinos = roundhalfup(get_sortino_ratio(trades_list['profit'], N, rf, ) * 100)
+    sortinos = roundup(get_sortino_ratio(trades_list['profit'], N, rf, ) * 100)
 
     df_perf = pd.concat([df_perf, pd.Series(
         ["Sortino Ratio", sortinos], index=cols[:2]).to_frame().T], ignore_index=True)
 
     # Calmar Ratios
     # calmars = roundup(trades_list['profit'].mean() * 255 / abs(trades_list['Drawdown'].max()))
 
@@ -449,37 +474,36 @@
         100 - (100 * (total_closed_trades_short - winning_trades_short) / total_closed_trades_short), 2)
     df_perf = pd.concat([df_perf, pd.Series(
         ["Percent Profitable", percent_profitable, np.nan, percent_profitable_long, np.nan, percent_profitable_short,
          np.nan],
         index=cols).to_frame().T], ignore_index=True)
 
     # Avg Trade
-    avg_trade = roundhalfup(trades_list['profit'].mean())
-    avg_trade_long = roundhalfup(trades_list[(trades_list['type'].str.contains('Long'))]['profit'].mean())
-    avg_trade_short = roundhalfup(trades_list[(trades_list['type'].str.contains('Short'))]['profit'].mean())
+    avg_trade = roundup(trades_list['profit'].mean())
+    avg_trade_long = roundup(trades_list[(trades_list['type'].str.contains('Long'))]['profit'].mean())
+    avg_trade_short = roundup(trades_list[(trades_list['type'].str.contains('Short'))]['profit'].mean())
     df_perf = pd.concat([df_perf, pd.Series(
         ["Avg Trade", avg_trade, None, avg_trade_long, np.nan, avg_trade_short, np.nan],
         index=cols).to_frame().T], ignore_index=True)
 
     # Avg Winning Trade
-    avg_winning_trade = roundhalfup(trades_list[(trades_list['profit'] > 0)]['profit'].mean())
-    avg_winning_trade_long = roundhalfup(
+    avg_winning_trade = roundup(trades_list[(trades_list['profit'] > 0)]['profit'].mean())
+    avg_winning_trade_long = roundup(
         trades_list[(trades_list['profit'] > 0) & (trades_list['type'].str.contains('Long'))]['profit'].mean())
-    avg_winning_trade_short = roundhalfup(
+    avg_winning_trade_short = roundup(
         trades_list[(trades_list['profit'] > 0) & (trades_list['type'].str.contains('Short'))]['profit'].mean())
     df_perf = pd.concat([df_perf, pd.Series(
         ["Avg Winning Trade", avg_winning_trade, np.nan, avg_winning_trade_long, np.nan, avg_winning_trade_short,
          np.nan],
         index=cols).to_frame().T], ignore_index=True)
 
     # Avg Losing Trade
-    avg_losing_trade = abs(roundhalfup(trades_list[(trades_list['profit'] < 0)]['profit'].mean()))
+    avg_losing_trade = abs(roundup(trades_list[(trades_list['profit'] < 0)]['profit'].mean()))
     avg_losing_trade_long = abs(
-        roundhalfup(
-            trades_list[(trades_list['profit'] < 0) & (trades_list['type'].str.contains('Long'))]['profit'].mean()))
-    avg_losing_trade_short = abs(roundhalfup(
+        roundup(trades_list[(trades_list['profit'] < 0) & (trades_list['type'].str.contains('Long'))]['profit'].mean()))
+    avg_losing_trade_short = abs(roundup(
         trades_list[(trades_list['profit'] < 0) & (trades_list['type'].str.contains('Short'))]['profit'].mean()))
     df_perf = pd.concat([df_perf, pd.Series(
         ["Avg Losing Trade", avg_losing_trade, np.nan, avg_losing_trade_long, np.nan, avg_losing_trade_short, np.nan],
         index=cols).to_frame().T], ignore_index=True)
 
     return df_perf
```

### Comparing `oakscript-0.0.1a0/setup.py` & `oakscript-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `oakscript-0.0.1a0/tests/strategies/rsi.py` & `oakscript-0.1.0/tests/strategies/rsi.py`

 * *Files identical despite different names*

