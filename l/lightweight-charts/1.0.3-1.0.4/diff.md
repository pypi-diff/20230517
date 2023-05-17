# Comparing `tmp/lightweight_charts-1.0.3.tar.gz` & `tmp/lightweight_charts-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightweight_charts-1.0.3.tar", last modified: Mon May 15 11:27:10 2023, max compression
+gzip compressed data, was "lightweight_charts-1.0.4.tar", last modified: Wed May 17 11:47:22 2023, max compression
```

## Comparing `lightweight_charts-1.0.3.tar` & `lightweight_charts-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-15 11:27:10.537022 lightweight_charts-1.0.3/
--rw-r--r--   0 louis      (501) staff       (20)     1066 2023-05-10 19:09:20.000000 lightweight_charts-1.0.3/LICENSE
--rw-r--r--   0 louis      (501) staff       (20)     5309 2023-05-15 11:27:10.536615 lightweight_charts-1.0.3/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)     4963 2023-05-15 11:26:26.000000 lightweight_charts-1.0.3/README.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-15 11:27:10.532447 lightweight_charts-1.0.3/lightweight_charts/
--rw-r--r--   0 louis      (501) staff       (20)       47 2023-05-14 13:49:11.000000 lightweight_charts-1.0.3/lightweight_charts/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)     8834 2023-05-15 11:19:36.000000 lightweight_charts-1.0.3/lightweight_charts/chart.py
--rw-r--r--   0 louis      (501) staff       (20)    22951 2023-05-14 16:01:34.000000 lightweight_charts-1.0.3/lightweight_charts/js.py
--rw-r--r--   0 louis      (501) staff       (20)   141259 2023-05-09 19:50:25.000000 lightweight_charts-1.0.3/lightweight_charts/pkg.py
--rw-r--r--   0 louis      (501) staff       (20)     2364 2023-05-12 11:50:34.000000 lightweight_charts-1.0.3/lightweight_charts/pywebview.py
--rw-r--r--   0 louis      (501) staff       (20)      516 2023-05-15 00:43:19.000000 lightweight_charts-1.0.3/lightweight_charts/qttest.py
--rw-r--r--   0 louis      (501) staff       (20)     1422 2023-05-10 00:01:10.000000 lightweight_charts-1.0.3/lightweight_charts/util.py
--rw-r--r--   0 louis      (501) staff       (20)     1721 2023-05-15 11:19:36.000000 lightweight_charts-1.0.3/lightweight_charts/widgets.py
--rw-r--r--   0 louis      (501) staff       (20)     1584 2023-05-14 13:53:44.000000 lightweight_charts-1.0.3/lightweight_charts/working.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-15 11:27:10.535941 lightweight_charts-1.0.3/lightweight_charts.egg-info/
--rw-r--r--   0 louis      (501) staff       (20)     5309 2023-05-15 11:27:10.000000 lightweight_charts-1.0.3/lightweight_charts.egg-info/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)      493 2023-05-15 11:27:10.000000 lightweight_charts-1.0.3/lightweight_charts.egg-info/SOURCES.txt
--rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-15 11:27:10.000000 lightweight_charts-1.0.3/lightweight_charts.egg-info/dependency_links.txt
--rw-r--r--   0 louis      (501) staff       (20)       17 2023-05-15 11:27:10.000000 lightweight_charts-1.0.3/lightweight_charts.egg-info/requires.txt
--rw-r--r--   0 louis      (501) staff       (20)       19 2023-05-15 11:27:10.000000 lightweight_charts-1.0.3/lightweight_charts.egg-info/top_level.txt
--rw-r--r--   0 louis      (501) staff       (20)       38 2023-05-15 11:27:10.537190 lightweight_charts-1.0.3/setup.cfg
--rw-r--r--   0 louis      (501) staff       (20)      609 2023-05-15 11:19:36.000000 lightweight_charts-1.0.3/setup.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-17 11:47:22.426091 lightweight_charts-1.0.4/
+-rw-r--r--   0 louis      (501) staff       (20)     1066 2023-05-10 19:09:20.000000 lightweight_charts-1.0.4/LICENSE
+-rw-r--r--   0 louis      (501) staff       (20)     5915 2023-05-17 11:47:22.425666 lightweight_charts-1.0.4/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)     5569 2023-05-16 14:49:40.000000 lightweight_charts-1.0.4/README.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-17 11:47:22.422606 lightweight_charts-1.0.4/lightweight_charts/
+-rw-r--r--   0 louis      (501) staff       (20)       47 2023-05-14 13:49:11.000000 lightweight_charts-1.0.4/lightweight_charts/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)     8733 2023-05-17 11:37:01.000000 lightweight_charts-1.0.4/lightweight_charts/chart.py
+-rw-r--r--   0 louis      (501) staff       (20)    23893 2023-05-17 11:40:17.000000 lightweight_charts-1.0.4/lightweight_charts/js.py
+-rw-r--r--   0 louis      (501) staff       (20)   141259 2023-05-09 19:50:25.000000 lightweight_charts-1.0.4/lightweight_charts/pkg.py
+-rw-r--r--   0 louis      (501) staff       (20)     1761 2023-05-17 11:00:03.000000 lightweight_charts-1.0.4/lightweight_charts/pywebview.py
+-rw-r--r--   0 louis      (501) staff       (20)     1753 2023-05-16 22:24:50.000000 lightweight_charts-1.0.4/lightweight_charts/util.py
+-rw-r--r--   0 louis      (501) staff       (20)     1949 2023-05-17 11:44:38.000000 lightweight_charts-1.0.4/lightweight_charts/widgets.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-17 11:47:22.425083 lightweight_charts-1.0.4/lightweight_charts.egg-info/
+-rw-r--r--   0 louis      (501) staff       (20)     5915 2023-05-17 11:47:22.000000 lightweight_charts-1.0.4/lightweight_charts.egg-info/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)      434 2023-05-17 11:47:22.000000 lightweight_charts-1.0.4/lightweight_charts.egg-info/SOURCES.txt
+-rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-17 11:47:22.000000 lightweight_charts-1.0.4/lightweight_charts.egg-info/dependency_links.txt
+-rw-r--r--   0 louis      (501) staff       (20)       17 2023-05-17 11:47:22.000000 lightweight_charts-1.0.4/lightweight_charts.egg-info/requires.txt
+-rw-r--r--   0 louis      (501) staff       (20)       19 2023-05-17 11:47:22.000000 lightweight_charts-1.0.4/lightweight_charts.egg-info/top_level.txt
+-rw-r--r--   0 louis      (501) staff       (20)       38 2023-05-17 11:47:22.426281 lightweight_charts-1.0.4/setup.cfg
+-rw-r--r--   0 louis      (501) staff       (20)      609 2023-05-17 11:46:48.000000 lightweight_charts-1.0.4/setup.py
```

### Comparing `lightweight_charts-1.0.3/LICENSE` & `lightweight_charts-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.3/PKG-INFO` & `lightweight_charts-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 Metadata-Version: 2.1
 Name: lightweight_charts
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python framework for TradingView's Lightweight Charts JavaScript library.
 Home-page: https://github.com/louisnw01/lightweight-charts-python
 Author: louisnw
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lightweight_charts_python
 
+[![PyPi Release](https://img.shields.io/pypi/v/lightweight-charts?color=32a852&label=PyPi)](https://pypi.org/project/lightweight-charts/)
+[![Made with Python](https://img.shields.io/badge/Python-3.9+-c7a002?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
+[![License](https://img.shields.io/github/license/louisnw01/lightweight-charts-python?color=9c2400)](https://github.com/louisnw01/lightweight-charts-python/blob/main/LICENSE)
+[![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
+
+
+
 
 lightweight-charts-python aims to provide a simple and pythonic way to access and implement [TradingView's Lightweight Charts](https://www.tradingview.com/lightweight-charts/).
 
 ## Installation
 ```
 pip install lightweight_charts
 ```
 ___
 
 ## Features
 1. Simple and easy to use.
 2. Blocking or non-blocking GUI.
 3. Streamlined for live data, with methods for updating directly from tick data.
-4. Support for wxPython.
+4. Support for PyQt and wxPython.
 ___
 
 ### 1. Display data from a csv:
 
 ```python
 import pandas as pd
 from lightweight_charts import Chart
@@ -205,17 +212,16 @@
     chart.subscribe_click(on_click)
 
     chart.show(block=True)
 
 ```
 ![callbacks gif](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/6_callbacks/callbacks.gif)
 ___
-## Wiki
 
-For a detailed guide of lightweight-charts-python, view the wiki [here](https://github.com/louisnw01/lightweight-charts-python/wiki).
+[![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
 
 ___
 
 _This package is an independent creation and has not been endorsed, sponsored, or approved by TradingView. The author of this package does not have any official relationship with TradingView, and the package does not represent the views or opinions of TradingView._
```

### Comparing `lightweight_charts-1.0.3/README.md` & `lightweight_charts-1.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 # lightweight_charts_python
 
+[![PyPi Release](https://img.shields.io/pypi/v/lightweight-charts?color=32a852&label=PyPi)](https://pypi.org/project/lightweight-charts/)
+[![Made with Python](https://img.shields.io/badge/Python-3.9+-c7a002?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
+[![License](https://img.shields.io/github/license/louisnw01/lightweight-charts-python?color=9c2400)](https://github.com/louisnw01/lightweight-charts-python/blob/main/LICENSE)
+[![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
+
+
+
 
 lightweight-charts-python aims to provide a simple and pythonic way to access and implement [TradingView's Lightweight Charts](https://www.tradingview.com/lightweight-charts/).
 
 ## Installation
 ```
 pip install lightweight_charts
 ```
 ___
 
 ## Features
 1. Simple and easy to use.
 2. Blocking or non-blocking GUI.
 3. Streamlined for live data, with methods for updating directly from tick data.
-4. Support for wxPython.
+4. Support for PyQt and wxPython.
 ___
 
 ### 1. Display data from a csv:
 
 ```python
 import pandas as pd
 from lightweight_charts import Chart
@@ -193,17 +200,16 @@
     chart.subscribe_click(on_click)
 
     chart.show(block=True)
 
 ```
 ![callbacks gif](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/6_callbacks/callbacks.gif)
 ___
-## Wiki
 
-For a detailed guide of lightweight-charts-python, view the wiki [here](https://github.com/louisnw01/lightweight-charts-python/wiki).
+[![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
 
 ___
 
 _This package is an independent creation and has not been endorsed, sponsored, or approved by TradingView. The author of this package does not have any official relationship with TradingView, and the package does not represent the views or opinions of TradingView._
```

### Comparing `lightweight_charts-1.0.3/lightweight_charts/chart.py` & `lightweight_charts-1.0.4/lightweight_charts/chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,14 @@
 from datetime import datetime
 from typing import Union
 
 from lightweight_charts.pywebview import _loop
 from lightweight_charts.util import LINE_TYPE, POSITION, SHAPE, CROSSHAIR_MODE, PRICE_SCALE_MODE
 
 
-# TODO Changelog
-#   Added support for PyQt.
-#   Refactored widgets to catch ModuleNotFoundErrors.
-
-
 class Line:
     def __init__(self, chart, line_id):
         self._chart = chart
         self.id = line_id
 
     def set(self, data: pd.DataFrame):
         """
```

### Comparing `lightweight_charts-1.0.3/lightweight_charts/js.py` & `lightweight_charts-1.0.4/lightweight_charts/js.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,81 @@
 import pandas as pd
 import uuid
 from datetime import timedelta, datetime
 from typing import Dict, Union
 
 from lightweight_charts.pkg import LWC_3_5_0
 from lightweight_charts.util import LINE_TYPE, POSITION, SHAPE, CROSSHAIR_MODE, _crosshair_mode, _line_type, \
-    MissingColumn, _js_bool, _price_scale_mode, PRICE_SCALE_MODE, _position, _shape
+    MissingColumn, _js_bool, _price_scale_mode, PRICE_SCALE_MODE, _position, _shape, IDGen
 
 
 class Line:
     def __init__(self, lwc, line_id, color, width):
         self._lwc = lwc
         self.loaded = False
         self.id = line_id
         self.color = color
         self.width = width
 
     def set(self, data: pd.DataFrame):
+        """
+        Sets the line data.\n
+        :param data: columns: date/time, price
+        """
         self._lwc._set_line_data(self.id, data)
 
     def update(self, series: pd.Series):
         """
         Updates the line data.\n
-        :param series: columns: date/time, price
+        :param series: labels: date/time, price
         """
         self._lwc._update_line_data(self.id, series)
 
 
+class API:
+    def __init__(self):
+        self.click_func = None
+
+    def onClick(self, data):
+        if isinstance(data['time'], int):
+            data['time'] = datetime.fromtimestamp(data['time'])
+        else:
+            data['time'] = datetime(data['time']['year'], data['time']['month'], data['time']['day'])
+        self.click_func(data) if self.click_func else None
+
+
 class LWC:
     def __init__(self, volume_enabled):
         self.js_queue = []
         self.loaded = False
         self._html = HTML
+        self._rand = IDGen()
+
+        self._js_api = API()
 
         self.volume_enabled = volume_enabled
         self.last_bar = None
         self.interval = None
         self._lines: Dict[uuid.UUID, Line] = {}
 
         self.background_color = '#000000'
         self.volume_up_color = 'rgba(83,141,131,0.8)'
         self.volume_down_color = 'rgba(200,127,130,0.8)'
 
-    def _on_js_load(self):
-        pass
+    def _on_js_load(self): pass
 
     def _stored(self, func, *args, **kwargs):
         if self.loaded:
             return False
         self.js_queue.append((func, args, kwargs))
         return True
 
-    def _set_last_bar(self, bar: pd.Series):
-        self.last_bar = bar
+    def _click_func_code(self, string): self._html = self._html.replace('// __onClick__', string)
+
+    def _set_last_bar(self, bar: pd.Series): self.last_bar = bar
 
     def _set_interval(self, df: pd.DataFrame):
         df['time'] = pd.to_datetime(df['time'])
         intervals = df['time'].diff()
         counts = intervals.value_counts()
         self.interval = counts.index[0]
 
@@ -78,16 +97,15 @@
         if self.interval != timedelta(days=1):
             string = string.timestamp()
             string = self.interval.total_seconds() * (string // self.interval.total_seconds())
         else:
             string = string.strftime('%Y-%m-%d')
         return string
 
-    def run_script(self, script):
-        pass
+    def run_script(self, script): pass
 
     def set(self, df: pd.DataFrame):
         """
         Sets the initial data for the chart.\n
         :param df: columns: date/time, open, high, low, close, volume (if volume enabled).
         """
         if self._stored('set', df):
@@ -128,15 +146,14 @@
 
             volume = series.drop(['open', 'high', 'low', 'close'])
             volume = volume.rename({'volume': 'value'})
             volume['color'] = self.volume_up_color if series['close'] > series['open'] else self.volume_down_color
             self.run_script(f'chart.volumeSeries.update({volume.to_dict()})')
             series = series.drop(['volume'])
 
-
         dictionary = series.to_dict()
         self.run_script(f'chart.series.update({dictionary})')
 
     def update_from_tick(self, series):
         """
         Updates the data from a tick.\n
         :param series: columns: date/time, price, volume (if volume enabled).
@@ -172,25 +189,27 @@
         return self._lines[line_id]
 
     def _set_line_data(self, line_id, df: pd.DataFrame):
         if self._stored('_set_line_data', line_id, df):
             return None
 
         line = self._lines[line_id]
+
         if not line.loaded:
+            var = self._rand.generate()
             self.run_script(f'''
-            let lineSeries = {{
+            let lineSeries{var} = {{
                     color: '{line.color}',
                     lineWidth: {line.width},
                     }};
-            let line = {{
-                series: chart.chart.addLineSeries(lineSeries),
+            let line{var} = {{
+                series: chart.chart.addLineSeries(lineSeries{var}),
                 id: '{line_id}',
             }};
-            lines.push(line)
+            lines.push(line{var})
                 ''')
             line.loaded = True
         df = self._df_datetime_format(df)
         self.run_script(f'''
         lines.forEach(function (line) {{
             if ('{line_id}' === line.id) {{
                 line.series.setData({df.to_dict('records')})
@@ -257,28 +276,29 @@
                         style: LINE_TYPE = 'solid', text: str = '', axis_label_visible=True):
         """
         Creates a horizontal line at the given price.\n
         """
         if self._stored('horizontal_line', price, color, width, style, text, axis_label_visible):
             return None
 
+        var = self._rand.generate()
         self.run_script(f"""
-               let priceLine = {{
+               let priceLine{var} = {{
                    price: {price},
                    color: '{color}',
                    lineWidth: {width},
                    lineStyle: LightweightCharts.LineStyle.{style},
                    axisLabelVisible: {'true' if axis_label_visible else 'false'},
                    title: '{text}',
                }};
-               let line = {{
-                   line: chart.series.createPriceLine(priceLine),
+               let line{var} = {{
+                   line: chart.series.createPriceLine(priceLine{var}),
                    price: {price},
                }};
-               horizontal_lines.push(line)""")
+               horizontal_lines.push(line{var})""")
 
     def remove_horizontal_line(self, price: Union[float, int]):
         """
         Removes a horizontal line at the given price.
         """
         if self._stored('remove_horizontal_line', price):
             return None
@@ -454,14 +474,21 @@
                   f'legendPercentVisible = {_js_bool(percent)}', f'legend.style.color = {color}', \
                   f'legend.style.fontSize = "{font_size}px"', f'legend.style.fontFamily = "{font_family}"'
         for script, arg in zip(scripts, (visible, ohlc, percent, color, font_size, font_family)):
             if arg is None:
                 continue
             self.run_script(script)
 
+    def subscribe_click(self, function: object):
+        if self._stored('subscribe_click', function):
+            return None
+
+        self._js_api.click_func = function
+        self.run_script('isSubscribed = true')
+
 
 SCRIPT = """
 
 const markers = []
 const horizontal_lines = []
 const lines = []
 
@@ -602,15 +629,15 @@
     let data = {
         time: param.time,
         open: prices.open,
         high: prices.high,
         low: prices.low,
         close: prices.close,
     }
-    pywebview.api.onClick(data)
+    // __onClick__
 
 }
 chart.chart.subscribeClick(clickHandler)
 """
 
 HTML = f"""
 <!DOCTYPE html>
```

### Comparing `lightweight_charts-1.0.3/lightweight_charts/pkg.py` & `lightweight_charts-1.0.4/lightweight_charts/pkg.py`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.3/lightweight_charts/pywebview.py` & `lightweight_charts-1.0.4/lightweight_charts/pywebview.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,24 @@
-import datetime
 import webview
 from multiprocessing import Queue
 
 from lightweight_charts.js import LWC
 
 _q = Queue()
 _result_q = Queue()
 
-DEBUG = True
-
-
-class API:
-    def __init__(self):
-        self.click_func = None
-
-    def onClick(self, data):
-        if isinstance(data['time'], int):
-            data['time'] = datetime.datetime.fromtimestamp(data['time'])
-        else:
-            data['time'] = datetime.datetime(data['time']['year'], data['time']['month'], data['time']['day'])
-        self.click_func(data) if self.click_func else None
-
 
 class Webview(LWC):
     def __init__(self, chart):
         super().__init__(chart.volume_enabled)
         self.chart = chart
         self.started = False
+        self._click_func_code('pywebview.api.onClick(data)')
 
-        self.js_api = API()
-        self.webview = webview.create_window('', html=self._html, on_top=chart.on_top, js_api=self.js_api,
+        self.webview = webview.create_window('', html=self._html, on_top=chart.on_top, js_api=self._js_api,
                                              width=chart.width, height=chart.height, x=chart.x, y=chart.y)
         self.webview.events.loaded += self._on_js_load
 
     def run_script(self, script): self.webview.evaluate_js(script)
 
     def _on_js_load(self):
         self.loaded = True
@@ -45,21 +30,14 @@
 
     def show(self):
         if self.loaded:
             self.webview.show()
         else:
             webview.start(debug=self.chart.debug)
 
-    def subscribe_click(self, function):
-        if self._stored('subscribe_click', function):
-            return None
-
-        self.js_api.click_func = function
-        self.run_script('isSubscribed = true')
-
     def create_line(self, color: str = 'rgba(214, 237, 255, 0.6)', width: int = 2):
         return super().create_line(color, width).id
 
     def hide(self): self.webview.hide()
 
     def exit(self):
         self.webview.destroy()
```

### Comparing `lightweight_charts-1.0.3/lightweight_charts/util.py` & `lightweight_charts-1.0.4/lightweight_charts/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from random import choices
+from string import ascii_lowercase
 from typing import Literal
 
 
 class MissingColumn(KeyError):
     def __init__(self, message):
         super().__init__(message)
         self.msg = message
@@ -54,8 +56,21 @@
 def _crosshair_mode(mode: CROSSHAIR_MODE): return mode.title() if mode else None
 
 
 def _js_bool(b: bool): return 'true' if b is True else 'false' if b is False else None
 
 
 def _price_scale_mode(mode: PRICE_SCALE_MODE):
-    return 'IndexedTo100' if mode == 'index100' else mode.title() if mode else None
+    return 'IndexedTo100' if mode == 'index100' else mode.title() if mode else None
+
+
+class IDGen:
+    def __init__(self):
+        self.list = []
+
+    def generate(self):
+        var = ''.join(choices(ascii_lowercase, k=8))
+        if var in self.list:
+            self.generate()
+        else:
+            self.list.append(var)
+            return var
```

### Comparing `lightweight_charts-1.0.3/lightweight_charts/widgets.py` & `lightweight_charts-1.0.4/lightweight_charts/widgets.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 try:
     import wx.html2
 except ImportError:
     pass
 try:
     from PyQt5.QtWebEngineWidgets import QWebEngineView
+    from PyQt5.QtWebChannel import QWebChannel
+    from PyQt5.QtCore import QObject
 except ImportError:
     pass
 
 from lightweight_charts.js import LWC
 
 
 class WxChart(LWC):
     def __init__(self, parent, volume_enabled=True):
-        super().__init__(volume_enabled)
         try:
-            self.webview = wx.html2.WebView.New(parent)
+            self.webview: wx.html2.WebView = wx.html2.WebView.New(parent)
         except NameError:
             raise ModuleNotFoundError('wx.html2 was not found, and must be installed to use WxChart.')
 
+        super().__init__(volume_enabled)
+
+        self.webview.AddScriptMessageHandler('wx_msg')
+        self._click_func_code('window.wx_msg.postMessage(data)')
+        self.webview.Bind(wx.html2.EVT_WEBVIEW_SCRIPT_MESSAGE_RECEIVED, lambda e: self._js_api.onClick(eval(e.GetString())))
+
         self.webview.Bind(wx.html2.EVT_WEBVIEW_LOADED, self._on_js_load)
         self.webview.SetPage(self._html, '')
 
-        self.second_load = False
-
     def run_script(self, script): self.webview.RunScript(script)
 
     def _on_js_load(self, e):
-        if not self.second_load:
-            self.second_load = True
-            return
         self.loaded = True
         for func, args, kwargs in self.js_queue:
             getattr(super(), func)(*args, **kwargs)
 
     def get_webview(self): return self.webview
 
 
 class QtChart(LWC):
     def __init__(self, widget=None, volume_enabled=True):
-        super().__init__(volume_enabled)
         try:
             self.webview = QWebEngineView(widget)
         except NameError:
             raise ModuleNotFoundError('QWebEngineView was not found, and must be installed to use QtChart.')
 
+        super().__init__(volume_enabled)
+
         self.webview.loadFinished.connect(self._on_js_load)
         self.webview.page().setHtml(self._html)
 
     def run_script(self, script): self.webview.page().runJavaScript(script)
 
     def _on_js_load(self):
         self.loaded = True
```

### Comparing `lightweight_charts-1.0.3/lightweight_charts.egg-info/PKG-INFO` & `lightweight_charts-1.0.4/lightweight_charts.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 Metadata-Version: 2.1
 Name: lightweight-charts
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python framework for TradingView's Lightweight Charts JavaScript library.
 Home-page: https://github.com/louisnw01/lightweight-charts-python
 Author: louisnw
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lightweight_charts_python
 
+[![PyPi Release](https://img.shields.io/pypi/v/lightweight-charts?color=32a852&label=PyPi)](https://pypi.org/project/lightweight-charts/)
+[![Made with Python](https://img.shields.io/badge/Python-3.9+-c7a002?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
+[![License](https://img.shields.io/github/license/louisnw01/lightweight-charts-python?color=9c2400)](https://github.com/louisnw01/lightweight-charts-python/blob/main/LICENSE)
+[![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
+
+
+
 
 lightweight-charts-python aims to provide a simple and pythonic way to access and implement [TradingView's Lightweight Charts](https://www.tradingview.com/lightweight-charts/).
 
 ## Installation
 ```
 pip install lightweight_charts
 ```
 ___
 
 ## Features
 1. Simple and easy to use.
 2. Blocking or non-blocking GUI.
 3. Streamlined for live data, with methods for updating directly from tick data.
-4. Support for wxPython.
+4. Support for PyQt and wxPython.
 ___
 
 ### 1. Display data from a csv:
 
 ```python
 import pandas as pd
 from lightweight_charts import Chart
@@ -205,17 +212,16 @@
     chart.subscribe_click(on_click)
 
     chart.show(block=True)
 
 ```
 ![callbacks gif](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/6_callbacks/callbacks.gif)
 ___
-## Wiki
 
-For a detailed guide of lightweight-charts-python, view the wiki [here](https://github.com/louisnw01/lightweight-charts-python/wiki).
+[![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
 
 ___
 
 _This package is an independent creation and has not been endorsed, sponsored, or approved by TradingView. The author of this package does not have any official relationship with TradingView, and the package does not represent the views or opinions of TradingView._
```

### Comparing `lightweight_charts-1.0.3/setup.py` & `lightweight_charts-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='lightweight_charts',
-    version='1.0.3',
+    version='1.0.4',
     packages=find_packages(),
     python_requires='>=3.9',
     install_requires=[
         'pandas',
         'pywebview',
     ],
     author='louisnw',
```

