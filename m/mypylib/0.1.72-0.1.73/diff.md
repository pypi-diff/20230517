# Comparing `tmp/mypylib-0.1.72.tar.gz` & `tmp/mypylib-0.1.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypylib-0.1.72.tar", last modified: Wed May 10 09:28:57 2023, max compression
+gzip compressed data, was "mypylib-0.1.73.tar", last modified: Wed May 17 12:30:57 2023, max compression
```

## Comparing `mypylib-0.1.72.tar` & `mypylib-0.1.73.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-10 09:28:57.217402 mypylib-0.1.72/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-05-10 09:28:57.217126 mypylib-0.1.72/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2022-08-12 06:28:20.000000 mypylib-0.1.72/README.md
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-10 09:28:57.213919 mypylib-0.1.72/mypylib/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2022-07-20 06:07:23.000000 mypylib-0.1.72/mypylib/MP_shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    46777 2023-05-10 09:27:59.000000 mypylib-0.1.72/mypylib/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2022-07-25 06:39:45.000000 mypylib-0.1.72/mypylib/binance_copy_bot.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     6342 2022-07-15 14:28:35.000000 mypylib-0.1.72/mypylib/binance_copy_bot_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2022-08-01 06:21:06.000000 mypylib-0.1.72/mypylib/chdbif.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2022-09-13 02:48:34.000000 mypylib-0.1.72/mypylib/crypto.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2022-08-12 06:28:16.000000 mypylib-0.1.72/mypylib/finmind.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2022-06-02 06:59:21.000000 mypylib-0.1.72/mypylib/libexcel.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    24230 2022-06-02 06:59:21.000000 mypylib-0.1.72/mypylib/mvp.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1255 2022-06-26 10:52:11.000000 mypylib-0.1.72/mypylib/mytest.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2022-06-12 10:26:49.000000 mypylib-0.1.72/mypylib/option_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2022-06-02 06:59:21.000000 mypylib-0.1.72/mypylib/shioaji_history_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-04-11 13:54:33.000000 mypylib-0.1.72/mypylib/shioaji_kline.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2022-06-02 06:59:21.000000 mypylib-0.1.72/mypylib/shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7649 2023-04-18 13:50:52.000000 mypylib-0.1.72/mypylib/sjtools.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2022-09-05 05:47:59.000000 mypylib-0.1.72/mypylib/tLineNotify.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7662 2022-06-02 06:59:21.000000 mypylib-0.1.72/mypylib/ti.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-10 09:28:57.216114 mypylib-0.1.72/mypylib/tmpDevelopment/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2022-07-16 06:27:26.000000 mypylib-0.1.72/mypylib/tmpDevelopment/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2022-07-16 07:09:42.000000 mypylib-0.1.72/mypylib/tmpDevelopment/warrant_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2543 2023-04-27 13:08:02.000000 mypylib-0.1.72/mypylib/tplaysound.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8467 2023-01-12 13:51:57.000000 mypylib-0.1.72/mypylib/tredis.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8184 2023-04-11 13:54:33.000000 mypylib-0.1.72/mypylib/warrant.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-10 09:28:57.215544 mypylib-0.1.72/mypylib.egg-info/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-05-10 09:28:56.000000 mypylib-0.1.72/mypylib.egg-info/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      654 2023-05-10 09:28:57.000000 mypylib-0.1.72/mypylib.egg-info/SOURCES.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2023-05-10 09:28:56.000000 mypylib-0.1.72/mypylib.egg-info/dependency_links.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2023-05-10 09:28:56.000000 mypylib-0.1.72/mypylib.egg-info/top_level.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2023-05-10 09:28:57.217512 mypylib-0.1.72/setup.cfg
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2022-06-29 14:27:00.000000 mypylib-0.1.72/setup.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-17 12:30:57.699808 mypylib-0.1.73/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-05-17 12:30:57.699568 mypylib-0.1.73/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2022-08-12 06:28:20.000000 mypylib-0.1.73/README.md
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-17 12:30:57.696797 mypylib-0.1.73/mypylib/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2022-07-20 06:07:23.000000 mypylib-0.1.73/mypylib/MP_shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    46835 2023-05-17 12:29:59.000000 mypylib-0.1.73/mypylib/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2022-07-25 06:39:45.000000 mypylib-0.1.73/mypylib/binance_copy_bot.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     6342 2022-07-15 14:28:35.000000 mypylib-0.1.73/mypylib/binance_copy_bot_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2022-08-01 06:21:06.000000 mypylib-0.1.73/mypylib/chdbif.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2022-09-13 02:48:34.000000 mypylib-0.1.73/mypylib/crypto.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2022-08-12 06:28:16.000000 mypylib-0.1.73/mypylib/finmind.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2022-06-02 06:59:21.000000 mypylib-0.1.73/mypylib/libexcel.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    24302 2023-05-17 12:28:48.000000 mypylib-0.1.73/mypylib/mvp.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1255 2022-06-26 10:52:11.000000 mypylib-0.1.73/mypylib/mytest.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2022-06-12 10:26:49.000000 mypylib-0.1.73/mypylib/option_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2022-06-02 06:59:21.000000 mypylib-0.1.73/mypylib/shioaji_history_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-04-11 13:54:33.000000 mypylib-0.1.73/mypylib/shioaji_kline.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2022-06-02 06:59:21.000000 mypylib-0.1.73/mypylib/shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7649 2023-04-18 13:50:52.000000 mypylib-0.1.73/mypylib/sjtools.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2022-09-05 05:47:59.000000 mypylib-0.1.73/mypylib/tLineNotify.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7316 2023-05-17 12:26:48.000000 mypylib-0.1.73/mypylib/ti.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-17 12:30:57.698763 mypylib-0.1.73/mypylib/tmpDevelopment/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2022-07-16 06:27:26.000000 mypylib-0.1.73/mypylib/tmpDevelopment/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2022-07-16 07:09:42.000000 mypylib-0.1.73/mypylib/tmpDevelopment/warrant_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2543 2023-04-27 13:08:02.000000 mypylib-0.1.73/mypylib/tplaysound.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8467 2023-01-12 13:51:57.000000 mypylib-0.1.73/mypylib/tredis.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8184 2023-04-11 13:54:33.000000 mypylib-0.1.73/mypylib/warrant.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-17 12:30:57.698247 mypylib-0.1.73/mypylib.egg-info/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-05-17 12:30:57.000000 mypylib-0.1.73/mypylib.egg-info/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      654 2023-05-17 12:30:57.000000 mypylib-0.1.73/mypylib.egg-info/SOURCES.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2023-05-17 12:30:57.000000 mypylib-0.1.73/mypylib.egg-info/dependency_links.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2023-05-17 12:30:57.000000 mypylib-0.1.73/mypylib.egg-info/top_level.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2023-05-17 12:30:57.699892 mypylib-0.1.73/setup.cfg
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2022-06-29 14:27:00.000000 mypylib-0.1.73/setup.py
```

### Comparing `mypylib-0.1.72/README.md` & `mypylib-0.1.73/README.md`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.72/mypylib/MP_shioaji_ticks.py` & `mypylib-0.1.73/mypylib/MP_shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.72/mypylib/__init__.py` & `mypylib-0.1.73/mypylib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import requests
 
 ssl._create_default_https_context = ssl._create_unverified_context
 from termcolor import cprint
 from inspect import currentframe
 
-__version__ = '0.1.72'
+__version__ = '0.1.73'
 
 __info__ = {
     '2022/01/04: 0.1.18 加入 __info__。',
     '2022/01/04: 0.1.18 Carey修改 MVP的部分。',
     '2022/01/05: 0.1.19 add check_place_cover 預防漲停鎖住',
     '2022/01/06: 0.1.20 add get_stock_future_data(). 用來抓取每天股票期貨資料',
     '2022/01/06: 0.1.20 add get_stock_future_snapshot(). 用來抓每天股票、股票期貨漲停、跌停價格',
@@ -60,15 +60,16 @@
     '2023/02/12: 0.1.65 修改 sjtools parse timestamp的方法，以免crash',
     '2023/02/13: 0.1.66 Move toggle_btn_off and toggle_btn_on here ',
     '2023/02/23: 0.1.67 get_new_warrant_list() 元富修改網站，封鎖 read_html()',
     '2023/03/15: 0.1.68 修正一些宣告',
     '2023/04/11: 0.1.69 換成shioaji 1.0 API',
     '2023/04/18: 0.1.70 Market() 增加 ask bid information',
     '2023/04/27: 0.1.71 tplaysound 減少buffer音量以免很吵',
-    '2023/05/10: 0.1.72 改用shioaji API'
+    '2023/05/10: 0.1.72 改用shioaji API',
+    '2023/05/17: 0.1.73 shioaji 1.0 改 Mmvp.py & ti.py'
 
 }
 
 request_headers = {
     'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'
 }
```

### Comparing `mypylib-0.1.72/mypylib/binance_copy_bot.py` & `mypylib-0.1.73/mypylib/binance_copy_bot.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.72/mypylib/binance_copy_bot_test.py` & `mypylib-0.1.73/mypylib/binance_copy_bot_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.72/mypylib/chdbif.py` & `mypylib-0.1.73/mypylib/chdbif.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.72/mypylib/crypto.py` & `mypylib-0.1.73/mypylib/crypto.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.72/mypylib/finmind.py` & `mypylib-0.1.73/mypylib/finmind.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.72/mypylib/libexcel.py` & `mypylib-0.1.73/mypylib/libexcel.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.72/mypylib/mvp.py` & `mypylib-0.1.73/mypylib/mvp.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                         'volume': []
                         }
 
     def period_accumulate(self, tick: Tick):
         # print(f'acc: {tick.ts} {tick.close} {tick.volume}')
         super().period_accumulate(tick)
 
-        self.mvp_tmp['ts'].append(tick.ts)
+        self.mvp_tmp['ts'].append(tick.datetime)
         self.mvp_tmp['close'].append(tick.close)
         self.mvp_tmp['volume'].append(tick.volume)
         self.volume_current = sum(self.mvp_tmp['volume'])
         if self.price_open == 0:
             self.price_open = tick.close
 
     def period_calculate(self, tick: Tick):
@@ -228,47 +228,47 @@
             cprint(f'{int(self.volume_moving / 1000)} volume low', 'blue')
             # return True
             return self.w.stop_trading_already
 
         if index < 6:
             return False
 
-        if False:
-            volume_burst = self.volume_burst
-            volume_lot = self.volume_lot
-            lot_buy = self.mvp_index.loc[self.mvp_index['lot'] == 1].shape[0]
-            lot_sell = self.mvp_index.loc[self.mvp_index['lot'] == -1].shape[0]
-            burst_buy = self.mvp_index.loc[self.mvp_index['burst'] == 1].shape[0]
-            burst_sell = self.mvp_index.loc[self.mvp_index['burst'] == -1].shape[0]
-            burst_count = self.mvp_index.iloc[2:].loc[self.mvp_index['volume'] >= volume_burst].shape[0]
-            lot_count = self.mvp_index.loc[self.mvp_index['volume'] >= volume_lot].shape[0]
-            last_burst_buy = self.mvp_index.iloc[-10:].loc[self.mvp_index['burst'] == 1].shape[0]
-            last_burst_sell = self.mvp_index.iloc[-10:].loc[self.mvp_index['burst'] == -1].shape[0]
-            price_min = self.mvp_index['low'].min()
-            if burst_count > 0 and burst_buy > -1 and burst_sell < 1 and price_min >= self.price_open * 0.99:
-                self.count_volume_burst = burst_count
-                self.index_price_enter = index
-                self.price_enter = self.mvp_index.iloc[index]['close']
-                return True
-                if burst_buy > 0 and burst_sell - burst_buy <= 0 and burst_count < 10:
-                    self.index_price_enter = index
-                    self.price_enter = self.mvp_index.iloc[index]['close']
-                    print(f'count:{burst_count} buy:{burst_buy} sell:{burst_sell}')
-                    return True
-                else:
-                    return self.w.stop_trading_already
-                if not self.bool_skip_burst:
-                    if burst_sell < burst_buy:
-                        if last_burst_sell > 0:
-                            self.bool_skip_burst = True
-                            return False
-                        cprint(f'symbol:{self.symbol},count:{burst_count}, buy:{burst_buy}, sell:{burst_sell}, last:{last_burst_buy}, burst:{self.volume_burst_30s}', 'red')
-                        return self.w.stop_trading_already
-            else:
-                return self.w.stop_trading_already
+        # if False:
+        #     volume_burst = self.volume_burst
+        #     volume_lot = self.volume_lot
+        #     lot_buy = self.mvp_index.loc[self.mvp_index['lot'] == 1].shape[0]
+        #     lot_sell = self.mvp_index.loc[self.mvp_index['lot'] == -1].shape[0]
+        #     burst_buy = self.mvp_index.loc[self.mvp_index['burst'] == 1].shape[0]
+        #     burst_sell = self.mvp_index.loc[self.mvp_index['burst'] == -1].shape[0]
+        #     burst_count = self.mvp_index.iloc[2:].loc[self.mvp_index['volume'] >= volume_burst].shape[0]
+        #     lot_count = self.mvp_index.loc[self.mvp_index['volume'] >= volume_lot].shape[0]
+        #     last_burst_buy = self.mvp_index.iloc[-10:].loc[self.mvp_index['burst'] == 1].shape[0]
+        #     last_burst_sell = self.mvp_index.iloc[-10:].loc[self.mvp_index['burst'] == -1].shape[0]
+        #     price_min = self.mvp_index['low'].min()
+        #     if burst_count > 0 and burst_buy > -1 and burst_sell < 1 and price_min >= self.price_open * 0.99:
+        #         self.count_volume_burst = burst_count
+        #         self.index_price_enter = index
+        #         self.price_enter = self.mvp_index.iloc[index]['close']
+        #         return True
+        #         if burst_buy > 0 and burst_sell - burst_buy <= 0 and burst_count < 10:
+        #             self.index_price_enter = index
+        #             self.price_enter = self.mvp_index.iloc[index]['close']
+        #             print(f'count:{burst_count} buy:{burst_buy} sell:{burst_sell}')
+        #             return True
+        #         else:
+        #             return self.w.stop_trading_already
+        #         if not self.bool_skip_burst:
+        #             if burst_sell < burst_buy:
+        #                 if last_burst_sell > 0:
+        #                     self.bool_skip_burst = True
+        #                     return False
+        #                 cprint(f'symbol:{self.symbol},count:{burst_count}, buy:{burst_buy}, sell:{burst_sell}, last:{last_burst_buy}, burst:{self.volume_burst_30s}', 'red')
+        #                 return self.w.stop_trading_already
+        #     else:
+        #         return self.w.stop_trading_already
 
         if bool_put:
             cur_mvp = self.mvp_index.iloc[index]
             pre1_mvp = self.mvp_index.iloc[index - 1]
             pre2_mvp = self.mvp_index.iloc[index - 3]
             pre3_mvp = self.mvp_index.iloc[index - 6]
             ts = cur_mvp['ts']
```

### Comparing `mypylib-0.1.72/mypylib/mytest.py` & `mypylib-0.1.73/mypylib/mytest.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.72/mypylib/option_test.py` & `mypylib-0.1.73/mypylib/option_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.72/mypylib/shioaji_history_ticks.py` & `mypylib-0.1.73/mypylib/shioaji_history_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.72/mypylib/shioaji_kline.py` & `mypylib-0.1.73/mypylib/shioaji_kline.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.72/mypylib/shioaji_ticks.py` & `mypylib-0.1.73/mypylib/shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.72/mypylib/sjtools.py` & `mypylib-0.1.73/mypylib/sjtools.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.72/mypylib/tLineNotify.py` & `mypylib-0.1.73/mypylib/tLineNotify.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.72/mypylib/ti.py` & `mypylib-0.1.73/mypylib/ti.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 import pandas as pd
 import datetime
 import os
 import plotly.express as px
 
 
-class Tick:
-    def __init__(self, tick_dict: dict):
-        self.index = 0
-        self.bool_simtrade: bool = False
-        self.ts: datetime.datetime = tick_dict.get('ts', datetime.datetime(year=2020, month=1, day=1, hour=9, minute=0, second=0))
-        self.close = tick_dict.get('close', 0)
-        self.volume = tick_dict.get('volume', 0)
-        self.price_ask = tick_dict.get('ask_price', 0)
-        self.price_bid = tick_dict.get('bid_price', 0)
-        self.volume_ask = tick_dict.get('ask_volume', 0)
-        self.volume_bid = tick_dict.get('bid_volume', 0)
+from shioaji import TickSTKv1 as Tick
+from shioaji import QuoteSTKv1 as Quote
+from typing import Union
+
 
 
 class Base_Technical_Indicator(object):
 
     values = {}
 
     @classmethod
@@ -94,67 +87,67 @@
         # 目前只是為了畫圖用
         self.dict_result = {'time': [],
                             'close': [],
                             'MA': [],
                             'AVL': []
                             }
 
-    def period_accumulate(self, tick: Tick):
+    def period_accumulate(self, tick: Union[Tick, Quote]):
         # 所有價格總和與次數，用來計算所有價格的平均
         self.price_acc_total += tick.close
         self.count_price_acc_total += 1
 
         # 無論是否在區間內外，都要加成這兩個數值。時間到就會 reset
         self.price_acc_period += tick.close
         self.count_price_acc_period += 1
 
-    def period_calculate(self, tick: Tick):
+    def period_calculate(self, tick: Union[Tick, Quote]):
 
         # AVL 使用開盤之後所有的價格來計算平均
         if self.count_price_acc_total != 0:
             self.array_AVL.insert(0, self.price_acc_total / self.count_price_acc_total)
 
         # MA 是使用這段區間內的價格來平均
         if self.count_price_acc_period != 0:
             self.array_MA.insert(0, self.price_acc_period / self.count_price_acc_period)
 
             self.price_acc_period = 0
             self.count_price_acc_period = 0
 
         # print(f'Append {tick.ts}, {self.time_next_tick_second}')
-        self.dict_result['time'].append(tick.ts)
+        self.dict_result['time'].append(tick.datetime)
         self.dict_result['close'].append(tick.close)
         self.dict_result['MA'].append(self.array_MA[0])
         self.dict_result['AVL'].append(self.array_AVL[0])
 
-    def push(self, tick: Tick):
+    def push(self, tick: Union[Tick, Quote]):
 
-        if tick.ts.time() < datetime.time(9, 0, 0):
+        if tick.datetime.time() < datetime.time(9, 0, 0):
             return
 
-        if tick.bool_simtrade:
+        if tick.simtrade == 1:
             return
 
-        self.price_ask = tick.price_ask if tick.price_ask != 0 else self.price_ask
-        self.price_bid = tick.price_bid if tick.price_bid != 0 else self.price_bid
-        self.volume_ask = tick.volume_ask if tick.volume_ask != 0 else self.volume_ask
-        self.volume_bid = tick.volume_bid if tick.volume_bid != 0 else self.volume_bid
+        self.price_ask = tick.ask_price[0] if tick.ask_price[0] != 0 else self.price_ask
+        self.price_bid = tick.bid_price[0] if tick.bid_price[0] != 0 else self.price_bid
+        self.volume_ask = tick.ask_volume[0] if tick.ask_volume[0] != 0 else self.volume_ask
+        self.volume_bid = tick.bid_volume[0] if tick.bid_volume[0] != 0 else self.volume_bid
 
         if tick.close == 0:
             return
 
         # 第一個成交的 tick 到來的時間
         if not self.bool_start_time_determined:
-            self.time_start = tick.ts.replace(hour=9, minute=0, second=0, microsecond=0)
+            self.time_start = tick.datetime.replace(hour=9, minute=0, second=0, microsecond=0)
             # print(f'Start time: {self.time_start}')
 
             # The very first tick is counted as first K
 
         # 第一個成交的 tick 到目前為止經過多少秒數
-        time_now_second = (tick.ts - self.time_start).seconds
+        time_now_second = (tick.datetime - self.time_start).seconds
 
         self.price_open = tick.close if self.price_open == -1 else self.price_open
 
         self.price_close = tick.close
 
         self.price_highest = tick.close if tick.close > self.price_highest else self.price_highest
         self.price_lowest = tick.close if tick.close < self.price_lowest else self.price_lowest
@@ -197,19 +190,19 @@
 
         # print(self.dict_result)
         df = pd.DataFrame.from_dict(self.dict_result).astype({'close': float, 'MA': float, 'AVL': float})
         fig = px.line(df, x='time', y=['close', 'MA', 'AVL'], title=f'{date} {symbol}')
         fig.show()
         # fig.write_image(filename)
 
-    def check_place_order(self, tick: Tick, price_threshold_trigger):
+    def check_place_order(self, tick: Union[Tick, Quote], price_threshold_trigger):
         return True
 
 
-    def check_place_cover(self, tick: Tick, price_threshold_trigger):
+    def check_place_cover(self, tick: Union[Tick, Quote], price_threshold_trigger):
         return True
 
 
 if __name__ == '__main__':
     import gzip
     import json
     from shioaji_ticks import shioaji_ticks
```

### Comparing `mypylib-0.1.72/mypylib/tmpDevelopment/warrant_test.py` & `mypylib-0.1.73/mypylib/tmpDevelopment/warrant_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.72/mypylib/tplaysound.py` & `mypylib-0.1.73/mypylib/tplaysound.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.72/mypylib/tredis.py` & `mypylib-0.1.73/mypylib/tredis.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.72/mypylib/warrant.py` & `mypylib-0.1.73/mypylib/warrant.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.72/mypylib.egg-info/SOURCES.txt` & `mypylib-0.1.73/mypylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.72/setup.py` & `mypylib-0.1.73/setup.py`

 * *Files identical despite different names*

