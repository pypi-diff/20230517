# Comparing `tmp/lk_logger-5.5.0-py3-none-any.whl.zip` & `tmp/lk_logger-5.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,27 @@
-Zip file size: 36317 bytes, number of entries: 24
+Zip file size: 36983 bytes, number of entries: 25
 -rw-r--r--  2.0 unx      592 b- defN 80-Jan-01 00:00 lk_logger/__init__.py
 -rw-r--r--  2.0 unx      591 b- defN 80-Jan-01 00:00 lk_logger/_print.py
 -rw-r--r--  2.0 unx     1672 b- defN 80-Jan-01 00:00 lk_logger/cache.py
 -rw-r--r--  2.0 unx     5487 b- defN 80-Jan-01 00:00 lk_logger/config.py
 -rw-r--r--  2.0 unx     1563 b- defN 80-Jan-01 00:00 lk_logger/console.py
 -rw-r--r--  2.0 unx     4503 b- defN 80-Jan-01 00:00 lk_logger/control.py
--rw-r--r--  2.0 unx     6440 b- defN 80-Jan-01 00:00 lk_logger/frame_info.py
--rw-r--r--  2.0 unx    11873 b- defN 80-Jan-01 00:00 lk_logger/logger.py
+-rw-r--r--  2.0 unx     6459 b- defN 80-Jan-01 00:00 lk_logger/frame_info.py
+-rw-r--r--  2.0 unx    13000 b- defN 80-Jan-01 00:00 lk_logger/logger.py
 -rw-r--r--  2.0 unx    10446 b- defN 80-Jan-01 00:00 lk_logger/markup.py
 -rw-r--r--  2.0 unx     6265 b- defN 80-Jan-01 00:00 lk_logger/message_builder.py
 -rw-r--r--  2.0 unx     9899 b- defN 80-Jan-01 00:00 lk_logger/message_formatter.py
 -rw-r--r--  2.0 unx     4034 b- defN 80-Jan-01 00:00 lk_logger/path_helper.py
 -rw-r--r--  2.0 unx     2559 b- defN 80-Jan-01 00:00 lk_logger/pipeline.py
 -rw-r--r--  2.0 unx       71 b- defN 80-Jan-01 00:00 lk_logger/scanner/__init__.py
 -rw-r--r--  2.0 unx     6247 b- defN 80-Jan-01 00:00 lk_logger/scanner/analyser.py
 -rw-r--r--  2.0 unx     1128 b- defN 80-Jan-01 00:00 lk_logger/scanner/const.py
 -rw-r--r--  2.0 unx     1780 b- defN 80-Jan-01 00:00 lk_logger/scanner/exceptions.py
 -rw-r--r--  2.0 unx     9594 b- defN 80-Jan-01 00:00 lk_logger/scanner/scanner.py
 -rw-r--r--  2.0 unx     3238 b- defN 80-Jan-01 00:00 lk_logger/scanner/symbols.py
 -rw-r--r--  2.0 unx    19638 b- defN 80-Jan-01 00:00 lk_logger/scanner/text_scanner.py
 -rw-r--r--  2.0 unx      491 b- defN 80-Jan-01 00:00 lk_logger/scanner/typehint.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 lk_logger-5.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx     4884 b- defN 80-Jan-01 00:00 lk_logger-5.5.0.dist-info/METADATA
-?rw-r--r--  2.0 unx     1921 b- defN 16-Jan-01 00:00 lk_logger-5.5.0.dist-info/RECORD
-24 files, 115004 bytes uncompressed, 33249 bytes compressed:  71.1%
+-rw-r--r--  2.0 unx      769 b- defN 80-Jan-01 00:00 lk_logger/shunt.py
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 lk_logger-5.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx     4884 b- defN 80-Jan-01 00:00 lk_logger-5.5.1.dist-info/METADATA
+?rw-r--r--  2.0 unx     1995 b- defN 16-Jan-01 00:00 lk_logger-5.5.1.dist-info/RECORD
+25 files, 116993 bytes uncompressed, 33803 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -57,17 +57,20 @@
 
 Filename: lk_logger/scanner/text_scanner.py
 Comment: 
 
 Filename: lk_logger/scanner/typehint.py
 Comment: 
 
-Filename: lk_logger-5.5.0.dist-info/WHEEL
+Filename: lk_logger/shunt.py
 Comment: 
 
-Filename: lk_logger-5.5.0.dist-info/METADATA
+Filename: lk_logger-5.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: lk_logger-5.5.0.dist-info/RECORD
+Filename: lk_logger-5.5.1.dist-info/METADATA
+Comment: 
+
+Filename: lk_logger-5.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lk_logger/__init__.py

```diff
@@ -17,8 +17,8 @@
 def __init():
     import traceback
     pipeline.add(traceback, bprint)
     setup(quiet=True)
 
 
 __init()
-__version__ = '5.5.0'
+__version__ = '5.5.1'
```

## lk_logger/frame_info.py

```diff
@@ -148,15 +148,15 @@
     @property
     def filepath(self) -> str:
         """
         notice: the returned value may be '<string>', '<unknown>' etc.
         """
         return self._frame.f_globals.get(
             '__file__', self._frame.f_code.co_filename
-        )
+        ).replace('\\', '/')
     
     @property
     def lineno(self) -> int:
         return self._frame.f_lineno
     
     @property
     def indentation(self) -> int:
```

## lk_logger/logger.py

```diff
@@ -1,76 +1,77 @@
-from __future__ import annotations
-
 import typing as t
 from atexit import register
 from collections import deque
 from inspect import currentframe
 from threading import Thread
 from time import sleep
 
 from rich.console import RenderableType
+from rich.text import Text
 from rich.traceback import Traceback
 
 from ._print import bprint
 from ._print import debug  # noqa
 from .cache import LoggingCache
 from .config import LoggingConfig
 from .console import con_print
 from .frame_info import FrameInfo
 from .markup import MarkMeaning
 from .markup import MarkupAnalyser
 from .markup import T as T0
 from .message_builder import MessageBuilder
 from .path_helper import path_helper
 from .pipeline import pipeline
+from .shunt import Shunt
+from .shunt import T as T1
 
 __all__ = ['LKLogger', 'lk']
 
 
 class _RawArgs:  # a workaround. see its usage below.
     def __init__(self, args: t.Tuple[t.Any, ...]):
         self.args = args
 
 
-class T(T0):  # Typehint
+class T:  # Typehint
     Args = t.Tuple[t.Any, ...]
+    Markup = T0.Markup
     MarkupPos = int  # -1, 0, 1
-    
-    # MessageQueue = t.List[
-    #     t.Tuple[t.Union[str, tuple], dict,
-    #             t.Optional[t.Callable]]
-    # ]
+    Pipe = T1.Pipe
+    PipeId = T1.PipeId
     
     Info = t.TypedDict('Info', {
         'file_path'      : str,
-        'line_number'    : str,
-        'is_external_lib': bool,
         'function_name'  : str,
+        'is_external_lib': bool,
+        'line_number'    : str,
         'variable_names' : t.Iterable[str],
     })
     
+    ComposedMessage = t.Union[str, RenderableType, Traceback, _RawArgs]
     FlushScheme = int
     #   0: no flush
     #   1: instant flush
     #   2: instant flush and drain
     #   3: wait for flush
-    ComposedMessage = t.Tuple[
-        t.Union[str, RenderableType, Traceback, _RawArgs],
-        FlushScheme
-    ]
 
 
 class LKLogger:
     
     def __init__(self):
         self._analyser = MarkupAnalyser()
         self._builder = MessageBuilder()
         self._cache = LoggingCache()
         self._config = LoggingConfig()
         
+        self._shunt = Shunt()
+        # self._shunt.add(con_print)
+        self.add_pipe = self._shunt.add
+        self.remove_pipe = self._shunt.remove
+        
         self._running = False
         self._message_queue = deque()
         register(self._stop_running)
         self._thread = Thread(target=self._start_running)
         self._thread.daemon = True
         self._thread.start()
     
@@ -88,48 +89,55 @@
             show_varnames=self._config.show_varnames,
         )
     
     @property
     def config(self) -> dict:
         return self._config.to_dict()
     
-    def _start_running(self):
+    def _start_running(self) -> None:
         
         def consume() -> None:
             msg: t.Union[str, tuple]
             kwargs: dict
             custom_print: t.Optional[t.Callable]
             
             for i in range(len(self._message_queue)):
                 msg, kwargs, custom_print = self._message_queue.popleft()
                 if custom_print:
                     # debug(custom_print, msg, kwargs)
                     kwargs.pop('file', None)
                     custom_print(*msg, **kwargs)
                 else:
                     con_print(msg, **kwargs)
+                    if self._shunt:
+                        self._shunt(self._purify(msg))
         
         self._running = True
         while self._running:
             if self._message_queue:
                 consume()
             else:
                 sleep(10E-3)
         else:
             consume()
     
-    def _stop_running(self):
+    def _stop_running(self) -> None:
         if self._config.clear_unfinished_stream:
             self._message_queue.clear()
         self._running = False
         self._thread.join()
     
     # -------------------------------------------------------------------------
     
-    def log(self, *args, _frame_info: FrameInfo = None, **kwargs) -> None:
+    def log(
+            self,
+            *args: t.Any,
+            _frame_info: FrameInfo = None,
+            **kwargs
+    ) -> None:
         if _frame_info is None:
             _frame_info = FrameInfo(currentframe().f_back)
         
         if (path := _frame_info.filepath) \
                 and (custom_print := pipeline.get(path)):
             if self._config.async_:
                 self._message_queue.append((args, kwargs, custom_print))
@@ -137,55 +145,79 @@
                 custom_print(*args, **kwargs)
             return
         
         msg, flush_scheme = self._build_message(_frame_info, *args)
         is_raw = isinstance(msg, _RawArgs)
         # debug(msg)
         
+        self._print(msg, flush_scheme, _is_raw=is_raw, **kwargs)
+    
+    def _print(
+            self,
+            msg: T.ComposedMessage,
+            flush_scheme: T.FlushScheme = 0,
+            _is_raw: bool = False,
+            **kwargs
+    ) -> None:
         if flush_scheme == 0:
             if self._config.async_:
-                if is_raw:
+                if _is_raw:
                     self._message_queue.append((msg.args, kwargs, bprint))
                 else:
                     self._message_queue.append((msg, kwargs, None))
             else:
-                if is_raw:
+                if _is_raw:
                     bprint(*msg.args, **kwargs)
                 else:
                     con_print(msg, **kwargs)
+                    if self._shunt:
+                        self._shunt(self._purify(msg))
         elif flush_scheme == 1:
             while self._message_queue:
                 sleep(10E-3)
-            if is_raw:
+            if _is_raw:
                 bprint(*msg.args, **kwargs)
             else:
                 con_print(msg, **kwargs)
+                if self._shunt:
+                    self._shunt(self._purify(msg))
         elif flush_scheme == 2:
             if skipped_count := len(self._message_queue):
                 self._message_queue.clear()
                 print(':frp', f'[red dim](... skipped '
                               f'{skipped_count} messages)[/]')
-            if is_raw:
+            if _is_raw:
                 bprint(*msg.args, **kwargs)
             else:
                 con_print(msg, **kwargs)
+                if self._shunt:
+                    self._shunt(self._purify(msg))
         elif flush_scheme == 3:
-            if is_raw:
+            if _is_raw:
                 bprint(*msg.args, **kwargs)
             else:
                 con_print(msg, **kwargs)
+                if self._shunt:
+                    self._shunt(self._purify(msg))
+    
+    @staticmethod
+    def _purify(msg: T.ComposedMessage) -> t.Optional[str]:
+        if isinstance(msg, str):
+            text = Text.from_markup(msg)
+            return text.plain
+        return None
     
     def fmt(self, _frame_info: FrameInfo = None, *args, **_) -> str:
         return str(self._build_message(
             _frame_info or FrameInfo(currentframe().f_back), *args
         )[0])
     
     def _build_message(
             self, frame_info: FrameInfo, *args
-    ) -> T.ComposedMessage:
+    ) -> t.Tuple[T.ComposedMessage, T.FlushScheme]:
         """
         return: (str message, bool is_flush, bool is_drain)
             flush: print the message immediately.
             drain: drain the message queue.
                 if drain is True, the flush must be True.
         """
         args, markup_pos, markup = \
@@ -285,15 +317,15 @@
         
         return self._builder.compose(
             args, marks_meaning, info
         ), flush_scheme
     
     def _extract_markup_from_arguments(
             self, frame_id: str, args: T.Args
-    ) -> tuple[T.Args, T.MarkupPos, T.Markup]:
+    ) -> t.Tuple[T.Args, T.MarkupPos, T.Markup]:
         """
         return: (args, markup_pos, markup)
             markup_pos: which position of `markup` in `args`.
                 0 not exists, 1 first place, -1 last place.
         """
         if (markup_pos := self._cache.get_markup_pos(frame_id)) is None:
             is_markup = self._analyser.is_valid_markup
```

## Comparing `lk_logger-5.5.0.dist-info/METADATA` & `lk_logger-5.5.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lk-logger
-Version: 5.5.0
+Version: 5.5.1
 Summary: Python advanced print with varnames.
 Home-page: https://github.com/likianta/lk-logger
 License: MIT
 Author: Likianta
 Author-email: likianta@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `lk_logger-5.5.0.dist-info/RECORD` & `lk_logger-5.5.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-lk_logger/__init__.py,sha256=7VxS7FvxYmqykzDr6p755ALsvfJkC7P7tlVlPNYx4wo,592
+lk_logger/__init__.py,sha256=rNWWBbG7CjrjrIvcU6S3tWlwu8hD1LDvzjKTEo17kZM,592
 lk_logger/_print.py,sha256=Q0WdJ-TxOcQy1aKxEgaxaCrixq9GdXqQVF7YTw-jELo,591
 lk_logger/cache.py,sha256=ayisqijEVWmUatnNqrooM8urR0hIAzYkzcJTUt_8248,1672
 lk_logger/config.py,sha256=mmM6x2vlR5setLz_5dhWKHzwL4tvY-oESsNDl5FOLr4,5487
 lk_logger/console.py,sha256=GSoFWXBybfNuF7S7b3_OJL70h52OSlTPnCbpay1pL60,1563
 lk_logger/control.py,sha256=Fk8o5aGjTAAxhJs6G1EvTUZ3ERvlQ13H-cpX_Mn5CSQ,4503
-lk_logger/frame_info.py,sha256=0_Z7lUW07JI7hLt_N59tYyhz96EJEdinMexQuWiAQEg,6440
-lk_logger/logger.py,sha256=iN3WiNWFSaPSaRmcZlf9-hJycKzCcZ2ZQLLod0XmhAI,11873
+lk_logger/frame_info.py,sha256=tkraucs-K_hCvtp9IB8dvLkuZ8wG8kAQt0swz8b2mZQ,6459
+lk_logger/logger.py,sha256=H4zRYxiOH0ngig-BoM8MS25yZog4ZDt7Nl6IHPSCkEw,13000
 lk_logger/markup.py,sha256=FIDjNJ-q-Fb3T2FDCjhMDwyUrkH1mdY5_nFE1bSze20,10446
 lk_logger/message_builder.py,sha256=Jj6YEmEbwjaiIXndS32vMToXBAfgHKXw3wDGdoqCCgI,6265
 lk_logger/message_formatter.py,sha256=lIdEoMdKDOfdduTq9wfKvL5Q7el9GQRMQeX4p63wu0k,9899
 lk_logger/path_helper.py,sha256=LAZOe5XK_51I0YPA6rUuY0_DKtaMtHyz52xcHqRbxY0,4034
 lk_logger/pipeline.py,sha256=bo-Z9367i2TxxJOCS5_Rk_6CFccFyJYgp3-uw9q9LzQ,2559
 lk_logger/scanner/__init__.py,sha256=er6nQAKVaYpdk30878kEDo5vKTSa6CzR-CdxNJiaODo,71
 lk_logger/scanner/analyser.py,sha256=tbI48nDcBPthZoD8jlnpap7S6FIHs4u8pUMQpsmh6r4,6247
 lk_logger/scanner/const.py,sha256=pRfHUK2huF2oLkd-ZpGtGUKQ2T4K3EnlSI0pUGGnp6Q,1128
 lk_logger/scanner/exceptions.py,sha256=G1wpgEIzTLLrD6Q_m0qGD85v5KnlPm3CV1ZxgvGCVd8,1780
 lk_logger/scanner/scanner.py,sha256=7Ase1WyHD87cBr4k9zYehe9LgL91r0L1_XlgKHg1_Eg,9594
 lk_logger/scanner/symbols.py,sha256=ibW1-n7Xigo9LvowUSn6dIrx-UmiJyuxN321bSCilSg,3238
 lk_logger/scanner/text_scanner.py,sha256=84ese30Bh-H1ZVxT0jcNhsTwM1nLDkZOrUO1LSdjV6k,19638
 lk_logger/scanner/typehint.py,sha256=Vr929B1w9UGiLVEMIJJIyE6gULjd_NxmNVpssyZW_JI,491
-lk_logger-5.5.0.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-lk_logger-5.5.0.dist-info/METADATA,sha256=z2HDlLwKkrNsVFmMYL5jFk9YTI-brfosEO92mLByhRc,4884
-lk_logger-5.5.0.dist-info/RECORD,,
+lk_logger/shunt.py,sha256=X3wqfprKLsmSUgZifte0Ao9CB7MDh2A45IqC1Gt8f2Y,769
+lk_logger-5.5.1.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+lk_logger-5.5.1.dist-info/METADATA,sha256=L2BsGbfZ3Y7Z7yfiJommeNb2iJzsvV3JIeav8BLF_KA,4884
+lk_logger-5.5.1.dist-info/RECORD,,
```

