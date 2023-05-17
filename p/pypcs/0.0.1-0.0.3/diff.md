# Comparing `tmp/pypcs-0.0.1.tar.gz` & `tmp/pypcs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pypcs-0.0.1.tar", last modified: Fri Mar 31 04:08:08 2023, max compression
+gzip compressed data, was "dist\pypcs-0.0.3.tar", last modified: Wed May 17 19:09:23 2023, max compression
```

## Comparing `pypcs-0.0.1.tar` & `pypcs-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 04:08:08.856333 pypcs-0.0.1/
--rw-rw-rw-   0        0        0    17096 2023-03-18 11:08:12.000000 pypcs-0.0.1/LICENSE
--rw-rw-rw-   0        0        0    10631 2023-03-31 04:08:08.856333 pypcs-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    10197 2023-03-31 03:41:06.000000 pypcs-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-31 04:08:08.834085 pypcs-0.0.1/pyPCS/
--rw-rw-rw-   0        0        0     3372 2023-03-30 20:34:59.000000 pypcs-0.0.1/pyPCS/__init__.py
--rw-rw-rw-   0        0        0    22206 2023-03-30 19:17:59.000000 pypcs-0.0.1/pyPCS/_basicData.py
--rw-rw-rw-   0        0        0     3019 2023-03-30 19:03:44.000000 pypcs-0.0.1/pyPCS/_player.py
-drwxrwxrwx   0        0        0        0 2023-03-31 04:08:08.836601 pypcs-0.0.1/pyPCS/basicGenerator/
--rw-rw-rw-   0        0        0      422 2023-03-30 16:40:17.000000 pypcs-0.0.1/pyPCS/basicGenerator/__init__.py
--rw-rw-rw-   0        0        0    10364 2023-03-30 19:17:59.000000 pypcs-0.0.1/pyPCS/basicGenerator/basic_generator.py
--rw-rw-rw-   0        0        0     7160 2023-03-17 20:41:45.000000 pypcs-0.0.1/pyPCS/chorder.py
--rw-rw-rw-   0        0        0      487 2023-03-31 04:01:39.000000 pypcs-0.0.1/pyPCS/classmethod_dec.py
-drwxrwxrwx   0        0        0        0 2023-03-31 04:08:08.840014 pypcs-0.0.1/pyPCS/piecesGenerator/
--rw-rw-rw-   0        0        0      154 2023-03-30 16:41:20.000000 pypcs-0.0.1/pyPCS/piecesGenerator/__init__.py
--rw-rw-rw-   0        0        0       62 2023-03-30 16:38:45.000000 pypcs-0.0.1/pyPCS/piecesGenerator/pieces_generator.py
-drwxrwxrwx   0        0        0        0 2023-03-31 04:08:08.847678 pypcs-0.0.1/pyPCS/series/
--rw-rw-rw-   0        0        0      614 2023-03-30 20:34:06.000000 pypcs-0.0.1/pyPCS/series/__init__.py
--rw-rw-rw-   0        0        0    11550 2023-03-30 19:17:59.000000 pypcs-0.0.1/pyPCS/series/funcs.py
--rw-rw-rw-   0        0        0    16586 2023-03-30 20:36:33.000000 pypcs-0.0.1/pyPCS/series/series1d.py
--rw-rw-rw-   0        0        0    19361 2023-03-31 03:39:47.000000 pypcs-0.0.1/pyPCS/series/series2d.py
--rw-rw-rw-   0        0        0     6761 2023-03-30 14:27:59.000000 pypcs-0.0.1/pyPCS/series/tree.py
-drwxrwxrwx   0        0        0        0 2023-03-31 04:08:08.853989 pypcs-0.0.1/pypcs.egg-info/
--rw-rw-rw-   0        0        0    10631 2023-03-31 04:08:08.000000 pypcs-0.0.1/pypcs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2023-03-31 04:08:08.000000 pypcs-0.0.1/pypcs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 04:08:08.000000 pypcs-0.0.1/pypcs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-03-31 04:08:08.000000 pypcs-0.0.1/pypcs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-31 04:08:08.000000 pypcs-0.0.1/pypcs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-31 04:08:08.856333 pypcs-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      679 2023-03-31 04:06:36.000000 pypcs-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.591319 pypcs-0.0.3/
+-rw-rw-rw-   0        0        0    17096 2023-05-08 05:43:04.000000 pypcs-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       51 2023-05-17 19:04:31.000000 pypcs-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    13272 2023-05-17 19:09:23.591319 pypcs-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    12880 2023-05-17 18:12:55.000000 pypcs-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.551424 pypcs-0.0.3/pyPCS/
+-rw-rw-rw-   0        0        0    83140 2023-05-17 06:28:12.000000 pypcs-0.0.3/pyPCS/ChordAttr.json
+-rw-rw-rw-   0        0        0     1656 2023-05-15 09:00:39.000000 pypcs-0.0.3/pyPCS/MidiInputHandler.py
+-rw-rw-rw-   0        0        0     3362 2023-05-14 17:34:03.000000 pypcs-0.0.3/pyPCS/__init__.py
+-rw-rw-rw-   0        0        0    23593 2023-05-16 14:33:37.000000 pypcs-0.0.3/pyPCS/_basicData.py
+-rw-rw-rw-   0        0        0     3020 2023-05-08 05:43:04.000000 pypcs-0.0.3/pyPCS/_player.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.553419 pypcs-0.0.3/pyPCS/basicGenerator/
+-rw-rw-rw-   0        0        0      364 2023-05-14 17:33:49.000000 pypcs-0.0.3/pyPCS/basicGenerator/__init__.py
+-rw-rw-rw-   0        0        0    10426 2023-05-08 05:43:04.000000 pypcs-0.0.3/pyPCS/basicGenerator/basicGenerator.py
+-rw-rw-rw-   0        0        0     7163 2023-05-08 05:43:04.000000 pypcs-0.0.3/pyPCS/chorder.py
+-rw-rw-rw-   0        0        0    45352 2023-05-17 14:15:11.000000 pypcs-0.0.3/pyPCS/circle_of_fifth.png
+-rw-rw-rw-   0        0        0      487 2023-05-08 05:43:04.000000 pypcs-0.0.3/pyPCS/classmethod_dec.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.555414 pypcs-0.0.3/pyPCS/piecesGenerator/
+-rw-rw-rw-   0        0        0      154 2023-05-08 05:43:04.000000 pypcs-0.0.3/pyPCS/piecesGenerator/__init__.py
+-rw-rw-rw-   0        0        0      299 2023-05-08 05:43:04.000000 pypcs-0.0.3/pyPCS/piecesGenerator/pieces_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.561397 pypcs-0.0.3/pyPCS/series/
+-rw-rw-rw-   0        0        0      653 2023-05-08 05:43:04.000000 pypcs-0.0.3/pyPCS/series/__init__.py
+-rw-rw-rw-   0        0        0    29983 2023-05-17 14:59:44.000000 pypcs-0.0.3/pyPCS/series/funcs.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.564390 pypcs-0.0.3/pyPCS/series/images/
+-rw-rw-rw-   0        0        0    69072 2023-05-17 17:44:21.000000 pypcs-0.0.3/pyPCS/series/images/cof_show.png
+-rw-rw-rw-   0        0        0    83930 2023-05-17 17:54:00.000000 pypcs-0.0.3/pyPCS/series/images/cofs_show.png
+-rw-rw-rw-   0        0        0    25430 2023-05-17 17:16:38.000000 pypcs-0.0.3/pyPCS/series/series1d.py
+-rw-rw-rw-   0        0        0    25167 2023-05-15 08:35:30.000000 pypcs-0.0.3/pyPCS/series/series2d.py
+-rw-rw-rw-   0        0        0     4833 2023-05-08 05:43:04.000000 pypcs-0.0.3/pyPCS/series/tree.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.571371 pypcs-0.0.3/pypcs.egg-info/
+-rw-rw-rw-   0        0        0    13272 2023-05-17 19:09:23.000000 pypcs-0.0.3/pypcs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1089 2023-05-17 19:09:23.000000 pypcs-0.0.3/pypcs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 19:09:23.000000 pypcs-0.0.3/pypcs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-05-17 19:09:23.000000 pypcs-0.0.3/pypcs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-17 19:09:23.000000 pypcs-0.0.3/pypcs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 19:09:23.591319 pypcs-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      808 2023-05-17 19:08:19.000000 pypcs-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.577395 pypcs-0.0.3/test/
+-rw-rw-rw-   0        0        0     2517 2023-05-16 13:00:44.000000 pypcs-0.0.3/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.580347 pypcs-0.0.3/test/basicGenerator/
+-rw-rw-rw-   0        0        0       26 2023-05-15 08:57:40.000000 pypcs-0.0.3/test/basicGenerator/__init__.py
+-rw-rw-rw-   0        0        0       12 2023-05-15 08:58:51.000000 pypcs-0.0.3/test/basicGenerator/test_basicGenerator.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.582342 pypcs-0.0.3/test/piecesGenerator/
+-rw-rw-rw-   0        0        0       99 2023-05-15 08:58:51.000000 pypcs-0.0.3/test/piecesGenerator/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-15 08:58:51.000000 pypcs-0.0.3/test/piecesGenerator/test_pieces_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.589323 pypcs-0.0.3/test/series/
+-rw-rw-rw-   0        0        0      352 2023-05-15 08:57:52.000000 pypcs-0.0.3/test/series/__init__.py
+-rw-rw-rw-   0        0        0     3679 2023-05-14 21:28:30.000000 pypcs-0.0.3/test/series/test_funcs.py
+-rw-rw-rw-   0        0        0    12028 2023-05-17 17:57:22.000000 pypcs-0.0.3/test/series/test_series1d.py
+-rw-rw-rw-   0        0        0     1994 2023-05-15 08:49:15.000000 pypcs-0.0.3/test/series/test_series2d.py
+-rw-rw-rw-   0        0        0     4833 2023-05-08 05:43:04.000000 pypcs-0.0.3/test/series/test_tree.py
+-rw-rw-rw-   0        0        0      474 2023-05-15 08:55:20.000000 pypcs-0.0.3/test/test_MidiInputHandler.py
+-rw-rw-rw-   0        0        0      430 2023-05-14 17:14:53.000000 pypcs-0.0.3/test/test_chorder.py
+-rw-rw-rw-   0        0        0        2 2023-05-14 17:15:00.000000 pypcs-0.0.3/test/test_classmethod_dec.py
+-rw-rw-rw-   0        0        0      271 2023-05-14 17:11:03.000000 pypcs-0.0.3/test/test_player.py
```

### Comparing `pypcs-0.0.1/LICENSE` & `pypcs-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.1/pyPCS/__init__.py` & `pypcs-0.0.3/pyPCS/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 """
-pypcs
+pyPCS
 =====
 (unfinished)
 
 Provides
-  1. Various class object of post-tonal music items
+  1. Various class object_ of post-tonal music items
   2. Easy transpositions over post-tonal music items
-  3. Random chord, series, segment generation
+  3. Random chord, series, pitch_class_series generation
 
     We are trying to make a powerful and professional post tonal music analyzing tool.
 
     As midi file regard C4 as 60, so in pypcs, we consider C4'pypcs pitch space as 60 instead of 0.
 
 How to use the documentation
 ----------------------------
 Documentation is available in two forms: docstrings provided
 with the code, and a loose standing reference guide, available from
 `github <https://github.com/JasonLee-p/pyPCS>`_.
-(might be uncompleted somewhere as it'pypcs unfinished)
+(might be uncompleted somewhere as it is unfinished)
 
 To import `pyPCS`::
 
   >>> import pyPCS
 
 Code snippets are indicated by three greater-than signs::
 
-  >>> x = 42
-  >>> x = x + 1
+  >>> x = 69
+  >>> x = x % 12
 
 Use the built-in ``help`` function to view a function'pypcs docstring::
 
   >>> # unfinished
   >>> help(pyPCS.PitchSegment)
   ... # doctest: +SKIP
 
 For some objects, ``np.info(obj)`` may provide additional help.  This is
-particularly true if you see the line "Help on ufunc object:" at the top
+particularly true if you see the line "Help on ufunc object_:" at the top
 of the help() page.  Ufuncs are implemented in C, not Python, for speed.
 The native Python help() does not know how to view their help, but our
 np.info() function does.
 
 To search for documents containing a keyword, do::
 
   >>> # unfinished
@@ -69,16 +69,16 @@
 
 
 Some naming regulations:
 ------------------------
 If an attribute end up with "group",
     it means that it'pypcs order is not in consideration.
 
-If an attribute end up with "segment",
-    it means that it'pypcs ordered and contains rhyme set.
+If an attribute end up with "pitch_class_series",
+    it means that it'pypcs ordered and contains pitch_class_series set.
 
 If an attribute end up with "series",
     it means that it'pypcs ordered and contains pitches' or pitch sets' duration.
 """
 
 from .series import PitchSegment, PitchClassSeries
 
@@ -86,17 +86,17 @@
 
 from .chorder import root_note_PH, mod12
 
 __all__ = [
     "play_note", "play_chord", "play_chord_set", "play_pitch_segment",  # _player
     "root_note_PH", "mod12"  # chorder
 ]
-from .series.series1d import PitchSeries, Rhyme, Chord, PitchClassSeries
-from .series.series2d import PitchSegment, PitchClassSegment, ContourSegment
-from .basicGenerator import get_segments_subsegment, counterpoint, random_relative_pitch_set, \
+from .series.series1d import PitchSeries, Rhythm, Chord, PitchClassSeries
+from .series.series2d import PitchSegment, ContourSegment
+from .basicGenerator import get_segments_subsegment, counterpoint, \
     randomChord, randomSegment, randomRhythm
 from .piecesGenerator import *
 
 __all__.extend(series.__all__)
 __all__.extend(basicGenerator.__all__)
 __all__.extend(piecesGenerator.__all__)
```

### Comparing `pypcs-0.0.1/pyPCS/_basicData.py` & `pypcs-0.0.3/pyPCS/_basicData.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 """
 This module defines some decorators,
 and stores the map between notes and value, chord name and chroma vectors, and so on.
 """
+import math
 
 
 # 打印函数运行的时间
 def _prt_func_time(func):
-
     def f(*args, **kwargs):
         from time import time
         st = time()
         _return = func(*args, **kwargs)
-        print("Time: \033[0;33m" + str(time()-st) + "pypcs\033[0m")
+        print("Time: \033[0;33m" + str(time() - st) + "pypcs\033[0m")
         return _return
+
     return f
 
 
 # 打印函数每运行一定次数的时间
 def _prt_funcs_time(times):
-
     def __prt_funcs_time(func):
         st = 0
         counter = 0
 
         def f(*args, **kwargs):
             from time import time
             nonlocal counter, st
             st = time() if counter == 0 else st
             counter += 1
             if counter == times:
-                print(time()-st)
+                print(time() - st)
                 counter = 0
             return func(*args, **kwargs)
+
         return f
+
     return __prt_funcs_time
 
 
 # 打印函数运行过的次数
 def _prt_func_run_num(func):
     counter = 0
 
     def f(*args, **kwargs):
         nonlocal counter
         counter += 1
         print(counter)
         return func(*args, **kwargs)
+
     return f
 
 
 value_note = {
     0: 'C', 1: '#C', 2: 'D', 3: '#D', 4: 'E', 5: 'F', 6: '#F', 7: 'G', 8: '#G', 9: 'A', 10: '#A', 11: 'B',
     # 第一行用于音级集和判断音名
     21: 'A0', 22: '#A0', 23: 'B0', 24: 'C1', 25: '#C1', 26: 'D1', 27: '#D1', 28: 'E1', 29: 'F1',
@@ -115,14 +118,20 @@
     'c5', '#c5', 'd5', '#d5', 'e5', 'f5', '#f5', 'g5', '#g5', 'a5', '#a5', 'b5',
     'c6', '#c6', 'd6', '#d6', 'e6', 'f6', '#f6', 'g6', '#g6', 'a6', '#a6', 'b6',
     'c7', '#c7', 'd7', '#d7', 'e7', 'f7', '#f7', 'g7', '#g7', 'a7', '#a7', 'b7', 'c8',
     'C', '#C', 'D', '#D', 'E', 'F', '#F', 'G', '#G', 'A', '#A', 'B',
     'c', '#c', 'd', '#d', 'e', 'f', '#f', 'g', '#g', 'a', '#a', 'b'
 ]
 
+
+ChordsAttributes = {
+
+}
+
+
 chords_chroma_vector = {
     #
     #                                             三和弦
     #
     # 大三和弦                                     index:
     'C': [1, 0, 0, 0, 1, 0, 0, 1, 0, 0, 0, 0],  # 12*0
     '#C': [0, 1, 0, 0, 0, 1, 0, 0, 1, 0, 0, 0],
@@ -383,15 +392,15 @@
     'G7sus4': [1, 0, 1, 0, 0, 1, 0, 1, 0, 0, 0, 0],
     'bA7sus4': [0, 1, 0, 1, 0, 0, 1, 0, 1, 0, 0, 0],
     'A7sus4': [0, 0, 1, 0, 1, 0, 0, 1, 0, 1, 0, 0],
     'bB7sus4': [0, 0, 0, 1, 0, 1, 0, 0, 1, 0, 1, 0],
     'B7sus4': [0, 0, 0, 0, 1, 0, 1, 0, 0, 1, 0, 1],
     #
     #                                               省略音九和弦：
-    # 大九和弦省略七音（或加九音）
+    # 大九和弦省略七音（或三和弦add9）
     'Cadd9': [1, 0, 1, 0, 1, 0, 0, 1, 0, 0, 0, 0],  # 7 + 12*19
     '#Cadd9': [0, 1, 0, 1, 0, 1, 0, 0, 1, 0, 0, 0],
     'Dadd9': [0, 0, 1, 0, 1, 0, 1, 0, 0, 1, 0, 0],
     '#Dadd9': [0, 0, 0, 1, 0, 1, 0, 1, 0, 0, 1, 0],
     'Eadd9': [0, 0, 0, 0, 1, 0, 1, 0, 1, 0, 0, 1],
     'Fadd9': [1, 0, 0, 0, 0, 1, 0, 1, 0, 1, 0, 0],
     '#Fadd9': [0, 1, 0, 0, 0, 0, 1, 0, 1, 0, 1, 0],
@@ -428,9 +437,31 @@
     'BM9,-5': [0, 1, 0, 1, 0, 0, 0, 0, 0, 0, 1, 1],
     # TODO: unfinished
 }
 
 # The circle of fifth value of a pitch-class.
 # 五度圈音级集和：
 note_cof_value = {0: 0, 1: -5, 2: 2, 3: -3, 4: 4, 5: -1, 6: 6, 7: 1, 8: -4, 9: 3, 10: -2, 11: 5}
+# 五度圈角度映射：
+note_cof_angle = {
+    0: math.pi * 7 / 12, 1: math.pi * 17 / 12, 2: math.pi / 4, 3: math.pi * 13 / 12, 4: -math.pi / 12, 5: math.pi * 3 / 4,
+    6: -math.pi*5/12, 7: math.pi * 5/12, 8: math.pi*5/4, 9: math.pi/12, 10: math.pi*11/12, 11: -math.pi*1/4}
 # 紧张度计算的音程预设值
 note_tension = {0: 0, 1: 32, 2: 8, 3: 4, 4: 2, 5: 1, 6: 16, 7: 1, 8: 2, 9: 4, 10: 8, 11: 32}
+# 泛音强度
+overtone_strength = {12: 0.85, 19: 0.825, 24: 0.8, 28: 0.75, 31: 0.7, 34: 0.6, 36: 0.6, 38: 0.5}
+# 音程和不协和度之间的关系
+interval_dissonance_t1 = {
+    0: 0,
+    1: 5.5, 2: 3.3, 3: 2, 4: 2.3, 5: 1.5, 6: 3, 7: 0.5, 8: 2.8, 9: 1, 10: 1.8, 11: 2.9, 12: 0,
+    13: 2.2, 14: 1.5, 15: 1, 16: 1.2, 17: 0.7, 18: 2, 19: 0, 20: 1.4, 21: 0.5, 22: 0.9, 23: 1.4, 24: 0,
+    25: 1, 26: 0, 27: 0.4, 28: 0, 29: 0.3, 30: 1, 31: 0, 32: 0.6, 33: 0.2, 34: 0.1, 35: 0.6, 36: 0,
+    37: 0.5, 38: 0, 39: 0.2, 40: 0, 41: 0.15, 42: 0.5, 43: 0, 44: 0.3, 45: 0.1, 46: 0, 47: 0.3, 48: 0
+}
+
+interval_dissonance_t2 = {
+    0: 0,
+    1: 5.5, 2: 3.3, 3: 2, 4: 2.3, 5: 1.5, 6: 3, 7: 0.5, 8: 2.8, 9: 1, 10: 1.8, 11: 2.9, 12: 0,
+    13: 3.2, 14: 2.1, 15: 1.3, 16: 1.4, 17: 1, 18: 2, 19: 0, 20: 1.8, 21: 0.7, 22: 1.2, 23: 2, 24: 0,
+    25: 1.6, 26: 1, 27: 0.6, 28: 0, 29: 0.7, 30: 1, 31: 0, 32: 0.9, 33: 0.35, 34: 0, 35: 1, 36: 0,
+    37: 0.5, 38: 0, 39: 0.2, 40: 0, 41: 0.15, 42: 0.5, 43: 0, 44: 0.3, 45: 0.1, 46: 0, 47: 0.3, 48: 0
+}
```

### Comparing `pypcs-0.0.1/pyPCS/_player.py` & `pypcs-0.0.3/pyPCS/_player.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     if _player_ is None:
         del _player
 
 
 def play_pitch_segment(_player, pitch_segment, bpm=80, instrument='Piano'):
     """
     :param _player: Pygame.midi.Output(int) variable.
-    :param pitch_segment: PitchSegment class object or a list of pitch list and duration list.
+    :param pitch_segment: PitchSegment class object_ or a list of pitch list and duration list.
     :param bpm: Beats per minutes.
     :param instrument: 'Piano' or 'Strings'
     :return: None
     """
     print("Playing...")
     # initialize
     if type(pitch_segment) is list:
```

### Comparing `pypcs-0.0.1/pyPCS/basicGenerator/basic_generator.py` & `pypcs-0.0.3/pyPCS/basicGenerator/basicGenerator.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,32 +11,32 @@
 
 style_group = ["smooth", "more doted notes", "triple"]
 
 
 # 该函数在P_c_s_T文件中也有。
 def get_segments_subsegment(ps, start_time, finish_time=None):
     """
-    :param ps: Pitch series
+    :param ps: Pitch segment
     :param start_time:Start time
     :param finish_time:Finish time
-    :return: If start time is equal to finish time or finish time is None, it returns a pitch'pypcs value(int),
-        else, it returns a new pitch series(list with two lists inside).
+    :return: If start time is equal to finish time or finish time is None, it returns a pitch's value(int),
+        else, it returns a new pitch segment(list with two lists inside).
     """
     start_time = float(start_time)
     finish_time = float(finish_time) if finish_time is not None else None
     # 判断传入变量是否合法：
     total_duration = sum([float(i) for i in ps[1]])
     if finish_time < start_time:
         raise ValueError("Finish time should be larger than start time.")
     if float(start_time) == total_duration:
         raise ValueError("Start time should be smaller than total duration.")
     if finish_time > total_duration:
         print(finish_time)
         print(start_time)
-        raise ValueError("Finish time should be smaller than the total duration of the pitch series.")
+        raise ValueError("Finish time should be smaller than the total duration of the pitch segment.")
     p_set = ps[0]
     duration_set = ps[1]
     result_ps = [[], []]  # 返回结果
     start_index = 0
     finish_index = 0
     d_counter = 0
     start_cou = False
@@ -164,33 +164,34 @@
     if total_duration not in range(1, 20):
         if total_duration not in [j + 0.5 for j in range(1, 20)]:
             raise ValueError("The total_duration should be a multiple of 0.5")
     if total_duration > 4 * note_num:
         raise ValueError("The total_duration is too large")
     if total_duration < note_num / 3:
         raise ValueError("The note_num is too large")
-    all_available_durations = [0.25, 1 / 3, 0.5, 2 / 3, 0.75, 1, 1.25, 4 / 3, 1.5, 5 / 3, 1.75, 2, 2.5, 3, 4]
-    smooth_ad = np.array([0.5, 1, 1.5, 2, 2.5, 3, 4])
+    all_available_durations = [0.25, 1 / 3, 0.5, 2 / 3, 0.75, 1, 1.25, 4 / 3, 1.5, 5 / 3, 1.75, 2, 2.5, 3, 4,
+                               0.33, 0.67, 1.33]
+    smooth_ad = np.array([0.25, 0.5, 0.75, 1, 1.5, 2, 2.5, 3, 4])
     m_do_n_ad = np.array([0.25, 0.5, 0.75, 1, 1.25, 1.5, 1.75, 2, 2.5, 3, 4])
     triple_ad = np.array([1 / 3, 2 / 3, 1, 4 / 3, 5 / 3, 2, 3, 4])
     avr_dur = total_duration / note_num  # 平均时值
     rhythm_set = []
     flag = True
     while flag:
         rhythm_set.clear()
 
         if style == "smooth":
             if note_num == total_duration:
                 return ['1'] * note_num
             for j in range(note_num - 1):
                 if note_num < total_duration:
-                    n = int(np.random.normal(loc=avr_dur, scale=avr_dur/2, size=None) + 0.5)
+                    n = int(np.random.normal(loc=avr_dur, scale=avr_dur, size=None) + 0.5)
                     rhythm_set.append(str(n)) if n > 0 else rhythm_set.append('1')
                 if note_num > total_duration:
-                    n = find_nearest(smooth_ad, np.random.normal(loc=avr_dur, scale=avr_dur/2, size=None))
+                    n = find_nearest(smooth_ad, np.random.normal(loc=avr_dur, scale=avr_dur, size=None))
                     rhythm_set.append(str(Fraction(n))) if n > 0 else rhythm_set.append('1/2')
 
         elif style == "more doted notes":
             for j in range(note_num - 1):
                 if j != 0:  # 模拟附点音符
                     if rhythm_set[-1] == '3/2' and avr_dur > 0.75:
                         rhythm_set.append('1/2')
@@ -228,19 +229,19 @@
     ds = randomRhythm(note_num, total_duration, style)
     ds = [str(d) for d in ds] if _type == 'str' else ds
     return [random_pitch_set, ds]
 
 
 if __name__ == "__main__":
     """
-    series = random_segment(4, 5, note_scale=4, first_note=64, style='smooth')
+    segment = random_segment(4, 5, note_scale=4, first_note=64, style='smooth')
 
-    for i in range(len(series[0])):
-        relative_pitch = str(series[0][i])
-        duration = str(series[1][i])
+    for i in range(len(segment[0])):
+        relative_pitch = str(segment[0][i])
+        duration = str(segment[1][i])
         print(relative_pitch + " " * (4 - len(relative_pitch)), end="")
         print(duration)
-    play_pitch_segment(None, series, bpm=120)
+    play_pitch_segment(None, segment, bpm=120)
     """
     segment = [[61, 62, 63, 64, 65, 66], [1, 2, 1, 1, 2, 1]]
     print(segment)
     counterpoint(segment, average_interval=2, counterpoint_p_num=4, new_pset_scale_from_origin=0)
```

### Comparing `pypcs-0.0.1/pyPCS/chorder.py` & `pypcs-0.0.3/pyPCS/chorder.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     for ii in range(len(c_itv)):
         if ii != len(c_itv) - 1 and c_itv[ii + 1] - c_itv[ii] == 1:
             output += 1
     return output
 
 
 # 色值计算需要五度圈关系
-def c_k_colour(interval):
+def chord_colour_k(interval):
     spans = []
     for n in interval:
         spans.append(note_cof_value[n])
     return np.mean(spans)
 
 
 # 五度圈跨度计算需要五度圈关系
@@ -207,16 +207,16 @@
                 pc_itv_dict[interval].append(note_g[k])
         possible_root = []
         # TODO: 算法不完善，需要引入权重
         for _interval in [7, 5, 4, 8, 3, 9]:
             for _pitch in pc_itv_dict[_interval]:
                 possible_root.append(_pitch)
         if len(pc_itv_dict[0]) > 2:
-            possible_root.append(_interval[0])
+            possible_root.append(note_g[0])
         if possible_root:
-            print("Possible roots:" + str(pc_itv_dict))
+            # print("Possible roots:" + str(pc_itv_dict))
             return min(possible_root)
         return pc_itv_dict
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `pypcs-0.0.1/pyPCS/series/series1d.py` & `pypcs-0.0.3/pyPCS/series/series1d.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 from __future__ import annotations
-from typing import List
+
+import json
+import os.path
+from typing import List, Union
 import numpy as _np
+from PIL import ImageTk
 
 import pyPCS.series.series2d as s2  # 避免循环调用错误，不使用from语法
-from ..chorder import c_span, c_k_colour, semitone_num, root_note_PH
-from .funcs import chord_type, to_pc_group, pc_to_circle_of_fifth_ns
-from .tree import SeriesTree, RhymeTree
+from .._player import play_chord
+from ..chorder import c_span, chord_colour_k, semitone_num, root_note_PH
+from .funcs import chord_type, to_pc_set, pc_to_circle_of_fifth_ns, tendentiousness, chord_dissonance, \
+    chord_colour_hua, chord_consonance_tian, chroma_vector, chord_colour_hua_from_chromaVector, \
+    get_chordConsonanceTian_from_chromaVector
+from .tree import SeriesTree, RhythmTree, PitchClassSeriesTree
 from .._basicData import note_value
 
 
+# from ..classmethod_dec import once_per_arg
+
+
 class PitchSeries:
     """
-        Any function that change the series list return a new object of a class (may not be PitchSegment):
+        Any function that change the series list return a new object_ of a class (may not be PitchSegment):
 
-        Pitch series contains a pitch set and a rhyme, various attributes and transformations are included in the class:
+        Pitch series contains a pitch set, various attributes and transformations are included in the class:
         Attributes:
             number of notes:
             duration:
             average pitch:
             tendentiousness:
 
         Transformations:
@@ -27,366 +37,582 @@
             retrograde Inversion:
             multiplication:
             rotation:
         """
 
     def __init__(self, series: List[int], new_tree=True, name=False, parent=None, __style=None):
         """
-        The first element of variable 'rhyme' is a pitch list while the second element is a duration list.
+        The first element of variable 'pitch_class_series' is a pitch list while the second element is a duration list.
         You are not supposed to use attributes start with "__" !
         :param series: Segment.
         :param new_tree: If you want to set a new tree of segments and set this one as the parent, set it as True
         """
 
         # 判断输入值是否合法
         judging = [True
                    if (type(int(ii)) is not int) else 0
                    for ii in series]
         if True in judging:
             raise ValueError("Invalid note format.")
 
+        self.series = series  # 音高
+
         if new_tree is True and name is True:
             raise ValueError("You shouldn't change '__name' default value.")
         elif new_tree is False and name is False:
             raise ValueError("You haven't set '__name', which is necessary when 'new_tree' is False.")
-        elif new_tree is True:
+        if new_tree:
             self.parent = None
-            self.name = input("Enter the name of the series tree:\n")
+            self.name = input(f"Enter the name of the PitchSeries{self.series} tree:\n")
             self.tree = SeriesTree(self)
         elif type(name) is str:  # 这时传入的tree_name应当是转换方法，也就是每一次变换之后返回的第三个值。
             self.parent = parent
             self.name = f'{self.parent.name}: {name}'
-            self.tree = SeriesTree.check_tree(parent)
-            self.tree.append_(parent, self)
+            self.tree = parent.tree
+            self.tree.append_(self.parent, self)
         else:
             raise ValueError("Invalid tree_name")
 
         self.style = __style
-        self.series = series  # 音高
         self.length = len(series)  # 获取音高列表的长度
         self.average = _np.mean(series)  # 计算平均音高
-        segment_result = tendentiousness([[series], ['1'] * self.length])  # 音高和密度的趋向性
+        segment_result = tendentiousness([series, ['1'] * self.length])  # 音高和密度的趋向性
         self.pitch_tend = segment_result[0]  # 音高趋向性
 
-    def __hash__(self):
-        return hash(self.series)
-
-    def __eq__(self, other):
-        return self.series == other.compared_segment
-
-    def __len__(self):
-        return len(self.series)
-
-    def __iter__(self):
-        return self.series
-
-    def __add__(self, add_pitch: int):
-        new_series = [new_pitch + add_pitch for new_pitch in self.series]
-        return PitchSeries(new_series,
-                           new_tree=False, parent=self, name=f"Transposition{add_pitch}")
-
-    def __sub__(self, sub_pitch: int):
-        new_series = [new_pitch - sub_pitch for new_pitch in self.series]
-        return PitchSeries(new_series,
-                           new_tree=False, parent=self, name=f"Transposition{12 - sub_pitch}")
-
-    def __mod__(self, number: int):
-        pass
-
-    def __getitem__(self, item):
-        return self.series[int(item)]
-
-    def __setitem__(self, key, value):
-        """
-        Variable *keys includes two element.
-        Variable "values" is two-element list.
-        """
-        new_pitch_set = self.series
-        new_pitch_set[key] = value
-        return PitchSeries(new_pitch_set,
-                           new_tree=self, parent=self, name=f"Reset pitch[{key}]{note_value[value]}")
-
-    def __reversed__(self):
-        new_series = reversed(self.series)
-        return PitchSeries(list(new_series)[:],
-                           new_tree=self, parent=self, name="Retrograde (with rhyme)")
-
-    # def get_pc_segment(self) -> Tuple[PitchClassSegment, PitchSegment, str]:
-    #     pitch_class_set = to_pc_group(self.series[:], ordered=True)
-    #     return PitchClassSegment([pitch_class_set], self.rhyme[:]), self, "Pitch class series"
-
-    def get_average(self) -> float:
-        return self.average
-
-    def get_pitch_tend(self) -> float:
-        return self.pitch_tend
+    def show(self):
+        print(self.series)
 
     def Transposition(self, add_pitch: int) -> PitchSeries:
         """
-        This function creates a Transposition transformation of self.
+        This function creates a new obj.
+
         :param add_pitch: Transposition num.
-        :return:
-        Transposed pitch_segment,
-        Original pitch_segment,
-        A string indicating that a Transposition has been made.
+        :return: Transposed new PitchSeries obj.
         """
         new_series = [new_pitch + int(add_pitch) for new_pitch in self.series]
         return PitchSeries(new_series,
-                           new_tree=self, parent=self, name=f"Transposition{add_pitch}")
+                           new_tree=False, parent=self, name=f"Transposition{add_pitch}")
 
     def Retrograde(self, add_pitch: int = 0) -> PitchSeries:
         """
-        This function creates a Retrograde transformation of self without changing the rhythm.
+        This function creates a new obj.
+
         :param add_pitch: Transposition num.
-        :return: Retrograded pitch_segment, Original pitch_segment, A string indicating that a Retrograde has been made.
+        :return: Retrograded new PitchSeries obj.
         """
-        new_series = list(reversed(self.series))[:]
+        new_series = reversed(self.series)
         if add_pitch == 0:
             return s2.PitchSegment(new_series,
-                                   new_tree=self, parent=self, name="Retrograde without rhyme")
+                                   new_tree=False, parent=self, name="Retrograde")
         new_series = [new_pitch + int(add_pitch) for new_pitch in new_series]
         return s2.PitchSegment(new_series,
-                               new_tree=self, parent=self, name=f"Retrograde{add_pitch}")
+                               new_tree=False, parent=self, name=f"Retrograde{add_pitch}")
 
     def Inversion(self, axes: int) -> PitchSeries:
         """
-        This function creates an Inversion transformation of self without changing the rhythm.
+        This function creates a new obj.
+
         :param axes: An int to invert each pitch in the set.
-        :return: Inverted pitch_segment, Original pitch_segment, A string indicating that an Inversion has been made.
+        :return: Inverted new PitchSeries obj.
         """
         new_series = [2 * axes - pitch for pitch in self.series]
         return PitchSeries(new_series,
-                           new_tree=self, parent=self, name=f"Inversion{axes}")
+                           new_tree=False, parent=self, name=f"Inversion{axes}")
 
     def RetrogradeInversion(self, axes: int) -> PitchSeries:
         """
-        This function creates a Retrograde then Inversion transformation of self with changed rhythm.
+        This function creates a new obj.
+
         :param axes: An int to invert each pitch in the set.
-        :return: Retrograde then Inversion pitch_segment, Original pitch_segment,
-        A string indicating that a RetrogradeInversion has been made.
+        :return: Retrograde new PitchSeries obj.
         """
         new_series = reversed([2 * axes - pitch for pitch in self.series])
         return PitchSeries(new_series,
-                           new_tree=self, parent=self, name=f"RetrogradeInversion{axes} (with rhyme)")
+                           new_tree=False, parent=self, name=f"RetrogradeInversion{axes}")
 
     def Rotation(self, num: int, add_pitch: int = 0) -> PitchSeries:
         """
-        This function creates a Rotation transformation of self without changing the rhythm.
+        This function creates a new obj.
+
         :param num: Rotation num
         :param add_pitch: Transposition num.
-        :return: Retrograded pitch_segment, Original pitch_segment, A string indicating that a Rotation has been made.
+        :return: Retrograded new PitchSeries obj.
         """
         if not 0 <= num < self.length:
             raise ValueError("The attribute 'num' should be smaller than length of the series.")
         new_series = [self.series[(ii + num) % self.length] for ii in range(self.length)]
         if add_pitch == 0:
             return PitchSeries(new_series[:],
-                               new_tree=self, parent=self, name=f"Rotation{num}")
+                               new_tree=False, parent=self, name=f"Rotation{num}")
         new_series = [new_pitch + int(add_pitch) for new_pitch in new_series]
         return PitchSeries(new_series[:],
-                           new_tree=self, parent=self, name=f"Rotation{num},T{add_pitch}")
+                           new_tree=False, parent=self, name=f"Rotation{num},T{add_pitch}")
 
     def play(self, pg_player=None, bpm=80, instrument='piano'):
         """
-        :param pg_player: Pygame.midi.Output(int) var. If you haven't set it, keep it None.
-        eg:
-        player = pygame.midi.output(0)
-        ps1.play(pg_player=player)
+        :param pg_player: Pygame.midi.Output(int). If you haven't set it, keep it None.
+            eg:
+            player = pygame.midi.output(0)
+            pSeg.play(pg_player=player)
         :param bpm: Beats per minutes.
         :param instrument: instrument.
         """
         from .._player import play_pitch_segment
         play_pitch_segment(pg_player, [self, ['1'] * self.length], instrument=instrument, bpm=bpm)
         del play_pitch_segment
 
+    def __hash__(self):
+        return hash(self.series)
+
+    def __eq__(self, other: Union[PitchSeries, list]):
+        if type(other) == list:
+            return self.series == other
+        else:
+            return self.series == other.series
+
+    def __len__(self):
+        return len(self.series)
+
+    def __iter__(self):
+        return self.series
+
+    def __add__(self, add_pitch: int):
+        new_series = [(new_pitch + add_pitch) % 12 for new_pitch in self.series]
+        return PitchSeries(new_series,
+                           new_tree=False, parent=self, name=f"Transposition{add_pitch}")
+
+    def __sub__(self, sub_pitch: int):
+        new_series = [(new_pitch - sub_pitch) % 12 for new_pitch in self.series]
+        return PitchSeries(new_series,
+                           new_tree=False, parent=self, name=f"Transposition{12 - sub_pitch}")
+
+    def __mod__(self, number: int):
+        pass
+
+    def __getitem__(self, item):
+        return self.series[int(item)]
+
+    def __setitem__(self, key, value):
+        new_pitch_set = self.series
+        new_pitch_set[key] = value
+        return PitchSeries(new_pitch_set,
+                           new_tree=False, parent=self, name=f"Reset pitch[{key}]{note_value[value]}")
+
+    def __reversed__(self):
+        new_series = reversed(self.series)
+        return PitchSeries(list(new_series)[:],
+                           new_tree=False, parent=self, name="Retrograde")
+
 
-class Rhyme:
-    def __init__(self, rhyme: List[str], new_tree=True, name=False, parent=None, __style=None):
+class Rhythm:
+    def __init__(self, rhythm: List[str], new_tree=True, name=False, parent=None, __style=None):
         """
-        The first element of variable 'series' is a pitch list while the second element is a duration list.
-        You are not supposed to use attributes start with "__" !
-        :param rhyme: Segment.
+        :param rhythm: beat list.
         :param new_tree: If you want to set a new tree of segments and set this one as the parent, set it as True
         """
 
         # 判断输入值是否合法
         judging = [True
                    if (type(ii) is not str and ('/' not in ii, len(ii) != 1)) else 0
-                   for ii in rhyme]
+                   for ii in rhythm]
         if True in judging:
             raise ValueError("Invalid duration format.")
 
+        self.rhythm = rhythm  # 时值
+
         if new_tree is True and name is True:
             raise ValueError("You shouldn't change '__name' default value.")
         elif new_tree is False and name is False:
             raise ValueError("You haven't set '__name', which is necessary when 'new_tree' is False.")
         elif new_tree is True:
             self.parent = None
-            self.name = input("Enter the name of the series tree:\n")
-            self.tree = RhymeTree(self)
+            self.name = input(f"Enter the name of the Rhythm{self.rhythm} tree:\n")
+            self.tree = RhythmTree(self)
         elif type(name) is str:  # 这时传入的tree_name应当是转换方法，也就是每一次变换之后返回的第三个值。
             self.parent = parent
             self.name = f'{self.parent.name}: {name}'
-            self.tree = RhymeTree.check_tree(parent)
+            self.tree = parent.tree
             self.tree.append_(parent, self)
         else:
             raise ValueError("Invalid tree_name")
 
         self.style = __style
-        self.rhyme = rhyme  # 时值
-        self.length = len(rhyme)  # 获取音高列表的长度
-        self.total_duration = _np.sum([float(eval(d)) for d in rhyme])  # 获取总时值
-        segment_result = tendentiousness([[60] * self.length, rhyme])  # 音高和密度的趋向性
+        self.length = len(rhythm)  # 获取音高列表的长度
+        self.total_duration = _np.sum([float(eval(d)) for d in rhythm])  # 获取总时值
+        segment_result = tendentiousness([[60] * self.length, rhythm])  # 音高和密度的趋向性
         self.rhythm_intensity_tend = segment_result[1]  # 密度趋向性
 
-    def __hash__(self):
-        return hash(self.rhyme)
-
-    def __eq__(self, other):
-        if type(other) is Rhyme:
-            return self.rhyme == other.rhyme
-        if type(other) is list[str]:
-            return self.rhyme == other
-
-    def __len__(self):
-        return len(self.rhyme)
-
-    def __iter__(self):
-        return self.rhyme
-
-    def __add__(self, add_beat: int):
-        pass
-
-    def __sub__(self, sub_beat: int):
-        pass
+    def show(self):
+        print(self.rhythm)
 
-    def __mod__(self, number: int):
-        pass
-
-    def __getitem__(self, item):
-        return self.rhyme[int(item)]
-
-    def __setitem__(self, key, value):
+    def Retrograde(self) -> Rhythm:
         """
-        Variable *keys includes two element.
-        Variable "values" is two-element list.
-        """
-        new_rhyme = self.rhyme
-        new_rhyme[key] = value
-        return Rhyme(new_rhyme,
-                     new_tree=True, parent=self, name=f"Reset rhyme[{key}]{note_value[value]}")
-
-    def __reversed__(self):
-        new_duration_set = reversed(self.rhyme)
-        return Rhyme(list(new_duration_set)[:],
-                     new_tree=self, parent=self, name="Retrograde (with rhyme)")
+        This function creates a new obj.
 
-    def get_rhythm_intensity_tend(self) -> float:
-        return self.rhythm_intensity_tend
-
-    def Retrograde(self) -> Rhyme:
-        """
-        This function creates a Retrograde transformation of self with changed rhythm.
-        :return: Retrograded pitch_segment, Original pitch_segment, A string indicating that a Retrograde has been made.
+        :return: New retrograded Rhythm obj.
         """
-        new_rhyme = list(reversed(self.rhyme))[:]
-        return Rhyme(new_rhyme,
-                     new_tree=self, parent=self, name=f"Retrograde")
+        new_rhyme = list(reversed(self.rhythm))[:]
+        return Rhythm(new_rhyme,
+                      new_tree=False, parent=self, name=f"Retrograde")
 
-    def Rotation(self, num: int) -> Rhyme:
+    def Rotation(self, num: int) -> Rhythm:
         """
-        This function creates a Rotation transformation of self with changed rhythm.
+        This function creates a new obj.
+
         :param num: Rotation num
-        :return: Retrograded pitch_segment, Original pitch_segment, A string indicating that a Rotation has been made.
+        :return: New rotated Rhythm obj.
         """
         if not 0 <= num < self.length:
             raise ValueError("The attribute 'num' should be smaller than length of the series.")
-        new_duration_set = [self.rhyme[(ii + num) % self.length] for ii in range(self.length)]
+        new_duration_set = [self.rhythm[(ii + num) % self.length] for ii in range(self.length)]
         return s2.PitchSegment(new_duration_set[:],
-                               new_tree=self, parent=self, name=f"Rotation{num}")
+                               new_tree=False, parent=self, name=f"Rotation{num}")
 
     def play(self, pg_player=None, bpm=80, instrument='piano'):
         """
         :param pg_player: Pygame.midi.Output(int) var. If you haven't set it, keep it None.
         eg:
         player = pygame.midi.output(0)
         ps1.play(pg_player=player)
         :param bpm: Beats per minutes.
         :param instrument: instrument.
         """
         from .._player import play_pitch_segment
-        play_pitch_segment(pg_player, [[69] * self.length, self.rhyme], instrument=instrument, bpm=bpm)
+        play_pitch_segment(pg_player, [[69] * self.length, self.rhythm], instrument=instrument, bpm=bpm)
         del play_pitch_segment
 
+    def __hash__(self):
+        return hash(self.rhythm)
+
+    def __eq__(self, other):
+        if type(other) is list:
+            return self.rhythm == other
+        return self.rhythm == other.rhythm
+
+    def __len__(self):
+        return len(self.rhythm)
+
+    def __iter__(self):
+        return self.rhythm
+
+    def __mod__(self, number: int):
+        pass
+
+    def __getitem__(self, item):
+        return self.rhythm[int(item)]
+
+    def __setitem__(self, key, value):
+        """
+        """
+        new_rhyme = self.rhythm
+        new_rhyme[key] = value
+        return Rhythm(new_rhyme,
+                      new_tree=True, parent=self, name=f"Reset pitch_class_series[{key}]{note_value[value]}")
+
+    def __reversed__(self):
+        new_duration_set = reversed(self.rhythm)
+        return Rhythm(list(new_duration_set)[:],
+                      new_tree=False, parent=self, name="Retrograde")
+
 
 class Chord:
+    """
+    Class Chord
+    ===========
+
+    """
+    from PIL import Image
+    all_chords = []
+    _abs_dir = os.path.dirname(__file__)
+    _pc2position = {
+        0: (250, 109), 7: (321, 128), 2: (372, 179), 9: (391, 250), 4: (372, 321), 11: (321, 372),
+        6: (250, 391), 1: (179, 372), 8: (128, 321), 3: (109, 250), 10: (128, 179), 5: (179, 128)
+    }
+    _im = Image.open(os.path.join(os.path.dirname(_abs_dir), 'circle_of_fifth.png'))
+
+    @staticmethod
+    def get_colourTian_from_chromaVector(cv):
+        return get_chordConsonanceTian_from_chromaVector(cv), \
+               chord_colour_hua_from_chromaVector(cv)
+
+    @staticmethod
+    def get_colourTian_from_chordName(chord_name):
+        _abs_dir = os.path.dirname(__file__)
+        with open(os.path.join(os.path.dirname(_abs_dir), 'ChordAttr.json'), 'r') as f:  # TODO: 相对路径
+            f = f.read()
+            chordsAttr = json.loads(f)
+        return chordsAttr[chord_name][1]
+
+    @staticmethod
+    def show_circle_of_fifths(*chord_obj, bg='Beige'):
+        import tkinter as tk
+        root = tk.Tk()
+        img = ImageTk.PhotoImage(Chord._im)
+        root.title("Chord circle of fifth")
+        root.configure(bg=bg, height=600, width=500)
+        root.iconphoto(True, img)
+        main_cv_with_sb = tk.Canvas()
+        for chord in chord_obj:
+            canvas = tk.Canvas(root, bg=bg, highlightthickness=0, height=600, width=500)
+            canvas.create_image(250, 250, image=img)
+            canvas.create_text(250, 535, text=chord.type, font=('Arial', 20), anchor='center')
+            # 根据和弦画点连线
+            for i in range(12):
+                if i in chord.pitch_class_group:
+                    canvas.create_oval(
+                        Chord._pc2position[i][0] - 9, Chord._pc2position[i][1] - 9,
+                        Chord._pc2position[i][0] + 9, Chord._pc2position[i][1] + 9,
+                        fill='firebrick', outline='firebrick')
+                else:
+                    canvas.create_oval(
+                        Chord._pc2position[i][0] - 5, Chord._pc2position[i][1] - 5,
+                        Chord._pc2position[i][0] + 5, Chord._pc2position[i][1] + 5,
+                        fill='black', outline='black')
+            # last_pc = _pc2position[self.pitch_class_group[0]]
+            # for pc in self.pitch_class_group[1:]:
+            #     canvas.create_line(
+            #         last_pc[0], last_pc[1], _pc2position[pc][0], _pc2position[pc][0], fill='firebrick', width=6)
+            #     last_pc = _pc2position[pc]
+            # canvas.create_line(
+            #     last_pc[0], last_pc[1],
+            #     _pc2position[self.pitch_class_group[0]][0], _pc2position[self.pitch_class_group[0]][0],
+            #     fill='firebrick', width=6)
+            canvas.pack(expand=True, side='left')
+        root.mainloop()
+
     def __init__(self, pitch_group):
+        pitch_group = sorted(pitch_group)
+        self.length = len(pitch_group)  # 获取音高列表的长度
         self.pitch_group = pitch_group
-        self.chord_type = chord_type(pitch_group)
-        self.pitch_class_group = to_pc_group(pitch_group)
-        self.span = c_span(to_pc_group(pitch_group))
-        self.k_colour = c_k_colour(to_pc_group(pitch_group))
-        self.semitone_num = semitone_num(to_pc_group(pitch_group))
+        self.pitch_class_group = sorted(to_pc_set(pitch_group))  # 会剔除重复的对象
+        self.chroma_vector = chroma_vector(self.pitch_class_group)
+        self.type = chord_type(pitch_group)
+        self.cof_span = c_span(to_pc_set(pitch_group))
+        self.semitone_num = semitone_num(to_pc_set(pitch_group))
         self.root_note = root_note_PH(pitch_group)
-
-    def pitch_group(self):
-        return self.pitch_group
-
-    def get_chord_type(self):
-        return self.chord_type
+        self.colour_k = chord_colour_k(to_pc_set(pitch_group))
+        self.colour_hua = chord_colour_hua(pitch_group)
+        self.consonance_tian = chord_consonance_tian(pitch_group)
+        self.dissonance = chord_dissonance(pitch_group)
+        self.colour_tian = self.consonance_tian, self.colour_hua
+        Chord.all_chords.append(self)
+        # if self.type == "Unable to recognize":
+        #     return
+        # if _len := len(str(self.dissonance)) == 4:
+        #     print(f"{self.type}:\ndissonance= {self.dissonance}, colour= {self.colour_hua}")
+        # elif _len == 3:
+        #     print(f"{self.type}:\ndissonance= {self.dissonance} , colour= {self.colour_hua}")
+        # elif _len == 1:
+        #     print(f"{self.type}:\ndissonance= {self.dissonance}   , colour= {self.colour_hua}")
 
     def get_pc_group(self):
         return PitchClassSeries(self.pitch_class_group)[:], self, "Pitch set group"
 
+    def show_circle_of_fifth(self, bg='Beige'):
+        import tkinter as tk
+
+        root = tk.Tk()
+        img = ImageTk.PhotoImage(Chord._im)
+        root.title(f"Chord {self.type}")
+        root.iconphoto(True, img)
+        root.configure(bg=bg, height=600, width=500)
+
+        canvas = tk.Canvas(root, bg=bg, highlightthickness=0, height=600, width=500)
+        canvas.create_image(250, 250, image=img)
+        canvas.create_text(250, 535, text=self.type, font=('Arial', 20), anchor='center')
+        # 根据和弦画点连线
+        for i in range(12):
+            if i in self.pitch_class_group:
+                canvas.create_oval(
+                    Chord._pc2position[i][0] - 9, Chord._pc2position[i][1] - 9,
+                    Chord._pc2position[i][0] + 9, Chord._pc2position[i][1] + 9,
+                    fill='firebrick', outline='firebrick')
+            else:
+                canvas.create_oval(
+                    Chord._pc2position[i][0] - 5, Chord._pc2position[i][1] - 5,
+                    Chord._pc2position[i][0] + 5, Chord._pc2position[i][1] + 5,
+                    fill='black', outline='black')
+        # last_pc = _pc2position[self.pitch_class_group[0]]
+        # for pc in self.pitch_class_group[1:]:
+        #     canvas.create_line(
+        #         last_pc[0], last_pc[1], _pc2position[pc][0], _pc2position[pc][0], fill='firebrick', width=6)
+        #     last_pc = _pc2position[pc]
+        # canvas.create_line(
+        #     last_pc[0], last_pc[1],
+        #     _pc2position[self.pitch_class_group[0]][0], _pc2position[self.pitch_class_group[0]][0],
+        #     fill='firebrick', width=6)
+        canvas.pack(expand=True)
+        root.mainloop()
+
+    def play(self, player):
+        play_chord(player, self.pitch_group)
+
+    def __len__(self):
+        return len(self.pitch_group)
+
     def __sub__(self, other):
         return _np.mean(self.pitch_group) - _np.mean(other.pitch_group)
 
     def __gt__(self, other):
         if _np.mean(self.pitch_group) > _np.mean(other.pitch_group):
             return True
 
     def __lt__(self, other):
         if _np.mean(self.pitch_group) < _np.mean(other.pitch_group):
             return True
 
+    def __iter__(self):
+        return self.pitch_group
+
+    def __hash__(self):
+        return hash(self.pitch_group)
+
     def __eq__(self, other):
         if _np.mean(self.pitch_group) == _np.mean(other.pitch_group):
             return self == other
 
 
 # 音级集合
 class PitchClassSeries:
-    # TODO: unfinished
-    def __init__(self, pitch_class_set):
-        # 为了防止每调用一次都计算函数，先把结果存进变量
-        cns = pc_to_circle_of_fifth_ns(pitch_class_set)
-        dcns = pc_to_circle_of_fifth_ns(pitch_class_set)[1]
-        self.pitch_class_set = pitch_class_set  # unordered
-        self.pitch_class_group = sorted(list(set(pitch_class_set)))  # sorted, without repeating.
-        self.cof_note_set = cns
-        self.default_cof_note_set = dcns
-
-    def __add__(self, cal_set):
-        """
-        :param cal_set: The set that you want to add to note set. It has to be as long as the note set.
-        """
-        result = []
-        if len(self.pitch_class_set) != len(cal_set):
-            raise RuntimeError("The cal_set's length should be equal to note set's length.")
-        else:
-            for ns in range(len(cal_set)):
-                result.append((self.pitch_class_set[ns] + cal_set[ns]) % 12)
-            return result
-
-    # 比较向位集，向位集的元素数量必须相等
-    def compare_cal_set(self, c_set1, c_set2):
-        result1 = []
-        result2 = []
-        if len(c_set1) == len(c_set2):
-            for ns in range(len(c_set1)):
-                result1.append((self.pitch_class_set[ns] + c_set1[ns]) % 12)
-            for ns in range(len(c_set2)):
-                result2.append((self.pitch_class_set[ns] + c_set2[ns]) % 12)
-            if result1 == result2:
-                return True
+    def __init__(
+            self, series: List[int],
+            new_tree=True, name=False, parent=None):
+        """
+        :param series: Series.
+        :param new_tree: If you want to set a new tree of segments and set this one as the parent, set it as True
+        """
+
+        if new_tree is True and name is True:
+            raise ValueError("You shouldn't change '__name' default value.")
+        elif new_tree is False and name is False:
+            raise ValueError("You haven't set '__name', which is necessary when 'new_tree' is False.")
+        elif new_tree is True:
+            self.parent = None
+            self.name = input("Enter the name of the PitchSegment tree:\n")
+            self.tree = PitchClassSeriesTree(self)
+        elif type(name) is str:  # 这时传入的tree_name应当是转换方法，也就是每一次变换之后返回的第三个值。
+            self.parent = parent
+            self.name = f'{self.parent.name}: {name}'
+            self.tree = parent.tree
+            self.tree.append_(parent, self)
         else:
-            raise RuntimeError("The compared two c_sets' length should be the same.")
+            raise ValueError("Invalid tree_name")
+        # TODO: 检查节奏和音集长度是否相等
+        self.series = series
+        self.length = len(self.series)  # 获取音高列表的长度
+
+    def show(self):
+        print(self.series)
+
+    def Transposition(self, add_pitch: int) -> PitchClassSeries:
+        """
+        This function creates a new obj.
+
+        :param add_pitch: Transposition num.
+        :return: Transposed new PitchClassSeries obj.
+        """
+        new_series = [(new_pitch + add_pitch) % 12 for new_pitch in self.series]
+        return PitchClassSeries(new_series,
+                                new_tree=False, parent=self, name=f"Transposition{add_pitch}")
+
+    def Retrograde(self, add_pitch: int = 0) -> PitchClassSeries:
+        """
+        This function creates a new obj.
+
+        :param add_pitch: Transposition num.
+        :return: Retrograded new PitchClassSeries obj.
+        """
+        new_series = reversed(self.series)
+        if add_pitch == 0:
+            return PitchClassSeries(new_series,
+                                    new_tree=False, parent=self, name="Retrograde")
+        new_series = [(new_pitch + int(add_pitch)) % 12 for new_pitch in new_series]
+        return PitchClassSeries(new_series,
+                                new_tree=False, parent=self, name=f"Retrograde{add_pitch}")
+
+    def Inversion(self, add: int) -> PitchClassSeries:
+        """
+        This function creates a new obj.
+
+        :param add: An int to invert each pitch in the set.
+        :return: Inverted new PitchClassSeries obj.
+        """
+        new_series = [(12 - pitch if pitch else 0) for pitch in self.series]
+        new_series = [(new_pitch + int(add)) % 12 for new_pitch in new_series]
+        return PitchClassSeries(new_series,
+                                new_tree=False, parent=self, name=f"T{add}Inversion")
+
+    def RetrogradeInversion(self, axes: int) -> PitchClassSeries:
+        """
+        This function creates a new obj.
+
+        :param axes: An int to invert each pitch in the set.
+        :return: Retrograde then Inversion new PitchClassSeries obj.
+        """
+        new_series = reversed([2 * axes - pitch for pitch in self.series])
+        return PitchClassSeries(
+            new_series, new_tree=False, parent=self, name=f"RetrogradeInversion{axes} (with pitch_class_series)")
+
+    def Rotation(self, num: int) -> PitchClassSeries:
+        """
+        This function creates a new obj.
+
+        :param num: Rotation num
+        :return: Retrograded new PitchClassSeries obj.
+        """
+        if not 0 <= num < self.length:
+            raise ValueError("The attribute 'num' should be smaller than length of the series.")
+        new_series = [self.series[(ii + num) % self.length] for ii in range(self.length)]
+        return PitchClassSeries(new_series[:],
+                                new_tree=False, parent=self, name=f"Rotation{num}")
+
+    def play(self, pg_player=None, bpm=80, instrument='piano'):
+        """
+        :param pg_player: Pygame.midi.Output(int) var. If you haven't set it, keep it None.
+        eg:
+        player = pygame.midi.output(0)
+        ps1.play(pg_player=player)
+        :param bpm: Beats per minutes.
+        :param instrument: instrument.
+        """
+        from .._player import play_pitch_segment
+        play_pitch_segment(pg_player, [self, ['1'] * self.length], instrument=instrument, bpm=bpm)
+        del play_pitch_segment
+
+    def __hash__(self):
+        return hash(self.series)
+
+    def __eq__(self, other):
+        return self.series == other.compared_segment
+
+    def __len__(self):
+        return len(self.series)
+
+    def __iter__(self):
+        return self.series
+
+    def __add__(self, add_pitch: int):
+        new_series = [new_pitch + add_pitch for new_pitch in self.series]
+        return PitchClassSeries(new_series,
+                                new_tree=False, parent=self, name=f"Transposition{add_pitch}")
+
+    def __sub__(self, sub_pitch: int):
+        new_series = [new_pitch - sub_pitch for new_pitch in self.series]
+        return PitchClassSeries(new_series,
+                                new_tree=False, parent=self, name=f"Transposition{12 - sub_pitch}")
+
+    def __mod__(self, number: int):
+        pass
+
+    def __getitem__(self, item):
+        return self.series[int(item)]
+
+    def __setitem__(self, key, value):
+        new_pitch_set = self.series
+        new_pitch_set[key] = value
+        return PitchClassSeries(new_pitch_set,
+                                new_tree=False, parent=self, name=f"Reset pitch[{key}]{note_value[value]}")
+
+    def __reversed__(self):
+        new_series = reversed(self.series)
+        return PitchClassSeries(list(new_series)[:],
+                                new_tree=False, parent=self, name="Retrograde (with pitch_class_series)")
```

### Comparing `pypcs-0.0.1/pyPCS/series/series2d.py` & `pypcs-0.0.3/pyPCS/series/series2d.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,308 @@
 """
 This module defines functions in Pitches-class Set Theory.
 
 """
 from __future__ import annotations
 
 import numpy as _np
-from typing import List, Tuple
+from typing import Tuple, Union
+from fractions import Fraction
 
-from .. import series  # 避免循环调用错误，不使用from语法
+import pyPCS.series.series1d as ps  # 避免循环调用错误，不使用from语法
 from .. import basicGenerator
 from ..classmethod_dec import once_per_arg
-from .tree import SegmentTree, SeriesTree, RhymeTree
+from .tree import SegmentTree, SeriesTree, RhythmTree
 from .funcs import *
 
 
 # 有序的音集（截段）
 class PitchSegment:
     """
-    Any function that change the series list return a new object of a class (may not be PitchSegment):
+    Any function that change the series list return a new object_ of a class (may not be PitchSegment):
 
-    Pitch series contains a pitch set and a rhyme, various attributes and transformations are included in the class:
+    Pitch series contains a pitch set and a pitch_class_series, various attributes and transformations are included in the class:
+    Attributes:
+        number of notes:
+        duration:
+        average pitch:
+        tendentiousness:
+
+    Transformations:
+        transposition:
+        retrograde:
+        Inversion:
+        retrograde Inversion:
+        multiplication:
+        rotation:
+    """
+
+    def __init__(
+            self, segment: Union[List[Union[ps.PitchSeries, ps.Rhythm]], List[List[int], list[str]]],
+            new_tree=True, name=False, parent=None, __style=None):
+        """
+        The first element of variable 'series' is a PitchSeries object_ while the second element is a Rhythm object_.
+        You are not supposed to use attributes start with "__" !
+        :param segment: Segment.
+        :param new_tree: If you want to set a new tree of segments and set this one as the parent, set it as True
+        """
+
+        if new_tree and name:
+            raise ValueError("You shouldn't change '__name' default value.")
+        elif new_tree is False and name is False:
+            raise ValueError("You haven't set '__name', which is necessary when 'new_tree' is False.")
+        elif new_tree:
+            self.parent = None
+            self.name = input("Enter the name of the PitchSegment tree:\n")
+            self.tree = SegmentTree(self)
+        elif type(name) is str:  # 这时传入的tree_name应当是转换方法，也就是每一次变换之后返回的第三个值。
+            self.parent = parent
+            self.name = f'{self.parent.name}: {name}'
+            self.tree = parent.tree
+            self.tree.append_(parent, self)
+        else:
+            raise ValueError("Invalid tree_name")
+        # TODO: 检查节奏和音集长度是否相等
+        self.pitchSeries = segment[0]  # 音集对象
+        self.rhythm = segment[1]  # 节奏对象
+        self.pitch_set = segment[0].series  # 音集列表
+        self.duration_set = segment[1].rhythm  # 节奏列表
+        self.segment = [self.pitch_set, self.duration_set]
+        self.style = __style
+        self.length = len(self.pitch_set)  # 获取音高列表的长度
+        self.total_duration = _np.sum([float(eval(d)) for d in self.duration_set])  # 获取总时值
+        self.w_average = pitches_weighed_average(self.segment)  # 计算加权（时值权重）平均音高
+        segment_result = tendentiousness(self.segment)  # 音高和密度的趋向性
+        self.pitch_tend = segment_result[0]  # 音高趋向性
+        self.rhythm_intensity_tend = segment_result[1]  # 密度趋向性
+
+    def show(self):
+        print(self.segment)
+
+    def show_sheet(self):
+        import matplotlib.pyplot as plt
+        # import matplotlib
+
+        # 设置图像大小和边距
+        fig = plt.figure(figsize=(8, 3), dpi=100)
+        plt.subplots_adjust(left=0.05, right=0.95, top=0.9, bottom=0.2)
+
+        # 绘制五条线
+        x = [0, 10]
+        for i in range(5):
+            y = [i * 2 + 1, i * 2 + 1]
+            plt.plot(x, y, 'k', linewidth=1)
+
+        # 显示图像
+        plt.axis('off')
+        plt.show()
+
+    @once_per_arg
+    def get_pc_segment(self) -> Tuple[object, PitchSegment, str]:
+        pitch_class_set = to_pc_set(self.pitch_set[:], ordered=True)
+        return ps.PitchClassSeries([pitch_class_set], self.rhythm), self, "Pitch class series"
+
+    def getSubsegment(self, start_beat, end_beat=None):
+        """
+        This attribute returns a pitch series list.
+
+        :param start_beat:Start beat.
+        :param end_beat:End beat.
+        :return:New PitchSegment object which is the subsegment of the original one.
+        """
+        s = get_subsegment(self.segment, start_beat, end_beat)[:]
+        return s
+
+    def getCounterpoint(self) -> PitchSegment:
+        """ Get a two voice series using counterpoint. """
+        # TODO:unfinished
+        print("getCounterpoint unfinished")
+        return self
+
+    def get_average(self) -> float:
+        return self.w_average
+
+    @once_per_arg
+    def Transposition(self, add_pitch: int) -> PitchSegment:
+        """
+        This function creates a Transposition transformation of self.
+
+        :param add_pitch: Transposition num.
+        :return: Transposed new PitchSegment object_.
+        """
+        new_ps = self.pitchSeries.Transposition(add_pitch)
+        return PitchSegment([new_ps, self.rhythm],
+                            new_tree=False, parent=self, name=f"Transposition{add_pitch % 12}")
+
+    @once_per_arg
+    def Retrograde_with_rhythm(self, add_pitch: int = 0) -> PitchSegment:
+        """
+        This function creates a Retrograde transformation of self with changed pitch_class_series.
+
+        :param add_pitch: Transposition num.
+        :return: Retrograded new PitchSegment object_.
+        """
+        new_ps = reversed(self.pitchSeries)
+        new_r = reversed(self.rhythm)
+        if add_pitch == 0:
+            return PitchSegment([new_ps, new_r],
+                                new_tree=False, parent=self, name="Retrograde (with pitch_class_series)")
+        new_ps_ = new_ps.Transposition(add_pitch)
+        return PitchSegment([new_ps_, new_r],
+                            new_tree=False, parent=self, name=f"Retrograde{add_pitch}")
+
+    @once_per_arg
+    def Retrograde_without_rhythm(self, add_pitch: int = 0) -> PitchSegment:
+        """
+        This function creates a Retrograde transformation of self without changing the pitch_class_series.
+        :param add_pitch: Transposition num.
+        :return: Retrograded new PitchSegment object_.
+        """
+        new_ps = reversed(self.pitchSeries)
+        if add_pitch == 0:
+            return PitchSegment([new_ps, self.rhythm],
+                                new_tree=False, parent=self, name="Retrograde (without pitch_class_series)")
+        new_ps_ = new_ps.Transposition(add_pitch)
+        return PitchSegment([new_ps_, self.rhythm],
+                            new_tree=False, parent=self, name=f"Retrograde{add_pitch} (without pitch_class_series)")
+
+    @once_per_arg
+    def Inversion(self, axes: int) -> PitchSegment:
+        """
+        This function creates an Inversion transformation of self without changing the pitch_class_series.
+        :param axes: An int to invert each pitch in the set.
+        :return: Inverted new PitchSegment object_.
+        """
+        new_ps = self.pitchSeries.Inversion(axes)
+        return PitchSegment([new_ps, self.rhythm],
+                            new_tree=False, parent=self, name=f"Inversion{axes}")
+
+    @once_per_arg
+    def RetrogradeInversion(self, axes: int) -> PitchSegment:
+        """
+        This function creates a Retrograde then Inversion transformation of self with changed pitch_class_series.
+        :param axes: An int to invert each pitch in the set.
+        :return: Retrograde then Inversion new PitchSegment object_.
+        """
+        new_ps_i = self.pitchSeries.Inversion(axes)
+        new_ps_ir = new_ps_i.Retrograde()
+        new_rhythm = reversed(self.rhythm)
+        return PitchSegment([new_ps_ir, new_rhythm],
+                            new_tree=False, parent=self, name=f"RetrogradeInversion{axes} (with pitch_class_series)")
+
+    @once_per_arg
+    def Rotation_without_rhythm(self, num: int, add_pitch: int = 0) -> PitchSegment:
+        """
+        This function creates a Rotation transformation of self without changing the pitch_class_series.
+        :param num: Rotation num
+        :param add_pitch: Transposition num.
+        :return: Roted new PitchSegment object_.
+        """
+        if not 0 <= num < self.length:
+            raise ValueError("The attribute 'num' should be smaller than length of the series.")
+        new_ps = self.pitchSeries.Rotation(num=num, add_pitch=add_pitch)
+        if add_pitch == 0:
+            return PitchSegment([new_ps, self.rhythm],
+                                new_tree=False, parent=self, name=f"Rotation{num} (without pitch_class_series)")
+        new_ps_ = new_ps.Transposition(add_pitch)
+        return PitchSegment([new_ps_, self.rhythm],
+                            new_tree=False, parent=self, name=f"Rotation{num} (without pitch_class_series),T{add_pitch}")
+
+    @once_per_arg
+    def Rotation_with_rhythm(self, num: int, add_pitch: int = 0) -> PitchSegment:
+        """
+        This function creates a Rotation transformation of self with changed pitch_class_series.
+        :param num: Rotation num
+        :param add_pitch: Transposition num.
+        :return: Retrograded new PitchSegment object_.
+        """
+        if not 0 <= num < self.length:
+            raise ValueError("The attribute 'num' should be smaller than length of the series.")
+        new_ps = self.pitchSeries.Rotation(num=num, add_pitch=add_pitch)
+        new_r = self.rhythm.Rotation(num)
+        if add_pitch == 0:
+            return PitchSegment([new_ps, new_r],
+                                new_tree=False, parent=self, name=f"Rotation{num} (with pitch_class_series)")
+        new_ps_ = new_ps.Transposition(add_pitch)
+        return PitchSegment([new_ps_, new_r],
+                            new_tree=False, parent=self, name=f"Rotation{num} (with pitch_class_series),T{add_pitch}")
+
+    def play(self, pg_player=None, bpm=80, instrument='piano'):
+        """
+        :param pg_player: Pygame.midi.Output(int) var. If you haven't set it, keep it None.
+        eg:
+        player = pygame.midi.output(0)
+        ps1.play(pg_player=player)
+        :param bpm: Beats per minutes.
+        :param instrument: instrument.
+        """
+        from .._player import play_pitch_segment
+        play_pitch_segment(pg_player, self.segment, instrument=instrument, bpm=bpm)
+        del play_pitch_segment
+
+    def __hash__(self):
+        return hash(self.segment)
+
+    def __eq__(self, other: Union[list, PitchSegment]):
+        if type(other) == list:
+            return self.segment == other
+        return self.segment == other.segment
+
+    def __len__(self):
+        return self.length
+
+    def __iter__(self):
+        return iter(zip(self.pitch_set, self.duration_set))
+
+    @once_per_arg
+    def __add__(self, add_pitch: int) -> PitchSegment:
+        new_ps = self.pitchSeries.Transposition(add_pitch)
+        return PitchSegment([new_ps, self.rhythm],
+                            new_tree=False, parent=self, name=f"Transposition{add_pitch}")
+
+    @once_per_arg
+    def __sub__(self, sub_pitch: int) -> PitchSegment:
+        new_ps = self.pitchSeries.Transposition(sub_pitch)
+        return PitchSegment([new_ps, self.rhythm],
+                            new_tree=False, parent=self, name=f"Transposition{12 - sub_pitch}")
+
+    def __mod__(self, number: int):
+        pass
+
+    def __getitem__(self, item):
+        return self.pitch_set[int(item)], self.duration_set[int(item)]
+
+    @once_per_arg
+    def __setitem__(self, key, value) -> PitchSegment:
+        """
+        Variable *keys includes two element.
+        Variable "values" is two-element list.
+        """
+        new_pitch_set = self.pitch_set
+        new_pitch_set[key] = value
+        new_pitch_series = ps.PitchSeries(
+            new_pitch_set, new_tree=False, parent=self.pitchSeries, name=f"Reset pitch[{key}]{note_value[value]}")
+        return PitchSegment(
+            [new_pitch_series, self.rhythm],
+            new_tree=False, parent=self, name=f"Reset pitch[{key}]{note_value[value]}")
+
+    @once_per_arg
+    def __reversed__(self) -> PitchSegment:
+        new_ps = reversed(self.pitchSeries)
+        new_r = reversed(self.rhythm)
+        return PitchSegment([new_ps, new_r],
+                            new_tree=False, parent=self, name="Retrograde (with pitch_class_series)")
+
+
+# 有序的音集（截段），这个是一个不实例化节奏和音级集合的版本，暂时不用
+class _PitchSegment:
+    """
+    Any function that change the series list return a new object_ of a class (may not be PitchSegment):
+
+    Pitch series contains a pitch set and a pitch_class_series, various attributes and transformations are included in the class:
     Attributes:
         number of notes:
         duration:
         average pitch:
         tendentiousness:
 
     Transformations:
@@ -69,91 +348,89 @@
             self.tree = SegmentTree.check_tree(parent)
             self.tree.append_(parent, self)
         else:
             raise ValueError("Invalid tree_name")
 
         self.segment = segment
         self.style = __style
-        self.pitch_set = segment[0]  # 音高
-        self.duration_set = segment[1]  # 时值
-        self.length = len(self.pitch_set)  # 获取音高列表的长度
-        self.total_duration = _np.sum([float(eval(d)) for d in self.duration_set])  # 获取总时值
+        self.pitch_series = segment[0]  # 音高
+        self.rhythm = segment[1]  # 时值
+        self.length = len(self.pitch_series)  # 获取音高列表的长度
+        self.total_duration = _np.sum([float(eval(d)) for d in self.rhythm])  # 获取总时值
         self.w_average = pitches_weighed_average(segment)  # 计算加权（时值权重）平均音高
         segment_result = tendentiousness(segment)  # 音高和密度的趋向性
         self.pitch_tend = segment_result[0]  # 音高趋向性
         self.rhythm_intensity_tend = segment_result[1]  # 密度趋向性
-        # 对时值表进行小数化，用于hash
-        ds = [round(eval(duration), 2) for duration in self.duration_set]
-        self.compared_segment = [self.pitch_set, ds[:]]
 
     def __hash__(self):
-        return hash(self.compared_segment)
+        return hash(self.segment)
 
     def __eq__(self, other):
-        return self.compared_segment == other.compared_segment
+        return self.segment == other.segment
 
     def __len__(self):
-        return len(self.duration_set)
+        return self.length
 
     def __iter__(self):
-        return iter(zip(self.pitch_set, self.duration_set))
+        return iter(zip(self.pitch_series, self.rhythm))
 
     @once_per_arg
     def __add__(self, add_pitch: int) -> PitchSegment:
-        new_pitch_set = [new_pitch + add_pitch for new_pitch in self.pitch_set]
-        return series.PitchSegment([new_pitch_set, self.duration_set][:],
-                                   new_tree=False, parent=self, name=f"Transposition{add_pitch}")
+        new_pitch_set = [new_pitch + add_pitch for new_pitch in self.pitch_series]
+        return PitchSegment([new_pitch_set, self.rhythm][:],
+                            new_tree=False, parent=self, name=f"Transposition{add_pitch}")
 
     @once_per_arg
     def __sub__(self, sub_pitch: int) -> PitchSegment:
-        new_pitch_set = [new_pitch - sub_pitch for new_pitch in self.pitch_set]
-        return series.PitchSegment([new_pitch_set, self.duration_set][:],
-                                   new_tree=False, parent=self, name=f"Transposition{12 - sub_pitch}")
+        new_pitch_set = [new_pitch - sub_pitch for new_pitch in self.pitch_series]
+        return PitchSegment([new_pitch_set, self.rhythm][:],
+                            new_tree=False, parent=self, name=f"Transposition{12 - sub_pitch}")
 
     def __mod__(self, number: int):
         pass
 
     def __getitem__(self, item):
-        return self.pitch_set[int(item)], self.duration_set[int(item)]
+        return self.pitch_series[int(item)], self.rhythm[int(item)]
 
     @once_per_arg
     def __setitem__(self, key, value) -> PitchSegment:
         """
         Variable *keys includes two element.
         Variable "values" is two-element list.
         """
-        new_pitch_set = self.pitch_set
+        new_pitch_set = self.pitch_series
         new_pitch_set[key] = value
-        return series.PitchSegment([new_pitch_set, self.duration_set[:]],
-                                   new_tree=self, parent=self, name=f"Reset pitch[{key}]{note_value[value]}")
+        return PitchSegment([new_pitch_set, self.rhythm[:]],
+                            new_tree=False, parent=self, name=f"Reset pitch[{key}]{note_value[value]}")
 
     @once_per_arg
     def __reversed__(self) -> PitchSegment:
-        new_pitch_set = reversed(self.pitch_set)
-        new_duration_set = reversed(self.duration_set)
-        return series.PitchSegment([list(new_pitch_set)[:], list(new_duration_set)[:]],
-                                   new_tree=self, parent=self, name="Retrograde (with rhyme)")
+        new_pitch_set = reversed(self.pitch_series)
+        new_duration_set = reversed(self.rhythm)
+        return PitchSegment([list(new_pitch_set)[:], list(new_duration_set)[:]],
+                            new_tree=False, parent=self, name="Retrograde (with pitch_class_series)")
 
     @once_per_arg
     def get_pc_segment(self) -> Tuple[object, PitchSegment, str]:
-        pitch_class_set = to_pc_group(self.pitch_set[:], ordered=True)
-        return series.PitchClassSegment([pitch_class_set], self.duration_set[:]), self, "Pitch class series"
+        pitch_class_set = to_pc_set(self.pitch_series[:], ordered=True)
+        import pyPCS.series.series1d as ps1
+        return ps1.PitchClassSeries([pitch_class_set], self.rhythm[:]), self, "Pitch class series"
 
     @once_per_arg
     def change_rhyme(self, total_duration: float, new_style: str) -> PitchSegment:
-        """ To overwrite a new rhyme to the pitch set.   """
+        """ To overwrite a new pitch_class_series to the pitch set.   """
         self.style = new_style
-        _segment = [self.pitch_set, basicGenerator.randomRhythm(self.length, total_duration, new_style)]
-        return series.PitchSegment(_segment,
-                                   new_tree=self, parent=self, __style=new_style, name="Different rhyme")
+        _segment = [self.pitch_series, basicGenerator.randomRhythm(self.length, total_duration, new_style)]
+        return PitchSegment(_segment,
+                            new_tree=False, parent=self, __style=new_style, name="Different pitch_class_series")
 
     def get_counterpoint(self) -> PitchSegment:
         """ Get a two voice series using counterpoint. """
         # TODO:unfinished
-        print("get_counterpoint unfinished")
+        print("getCounterpoint unfinished")
         return self
 
     def get_average(self) -> float:
         return self.w_average
 
     def get_pitch_tend(self) -> float:
         return self.pitch_tend
@@ -162,110 +439,110 @@
         return self.rhythm_intensity_tend
 
     @once_per_arg
     def Transposition(self, add_pitch: int) -> PitchSegment:
         """
         This function creates a Transposition transformation of self.
         :param add_pitch: Transposition num.
-        :return: Transposed new PitchSegment object.
+        :return: Transposed new PitchSegment object_.
         """
-        new_pitch_set = [new_pitch + int(add_pitch) for new_pitch in self.pitch_set]
-        return series.PitchSegment([new_pitch_set, self.duration_set][:],
-                                   new_tree=self, parent=self, name=f"Transposition{add_pitch%12}")
+        new_pitch_set = [new_pitch + int(add_pitch) for new_pitch in self.pitch_series]
+        return PitchSegment([new_pitch_set, self.rhythm][:],
+                            new_tree=False, parent=self, name=f"Transposition{add_pitch % 12}")
 
     @once_per_arg
     def Retrograde_with_rhyme(self, add_pitch: int = 0) -> PitchSegment:
         """
-        This function creates a Retrograde transformation of self with changed rhythm.
+        This function creates a Retrograde transformation of self with changed pitch_class_series.
         :param add_pitch: Transposition num.
-        :return: Retrograded new PitchSegment object.
+        :return: Retrograded new PitchSegment object_.
         """
-        new_pitch_set = list(reversed(self.pitch_set))[:]
-        new_duration_set = list(reversed(self.duration_set))[:]
+        new_pitch_set = list(reversed(self.pitch_series))[:]
+        new_duration_set = list(reversed(self.rhythm))[:]
         if add_pitch == 0:
-            return series.PitchSegment([new_pitch_set, new_duration_set],
-                                       new_tree=self, parent=self, name="Retrograde (with rhyme)")
+            return PitchSegment([new_pitch_set, new_duration_set],
+                                new_tree=False, parent=self, name="Retrograde (with pitch_class_series)")
         new_pitch_set = [new_pitch + int(add_pitch) for new_pitch in new_pitch_set]
-        return series.PitchSegment([new_pitch_set, new_duration_set],
-                                   new_tree=self, parent=self, name=f"Retrograde{add_pitch}")
+        return PitchSegment([new_pitch_set, new_duration_set],
+                            new_tree=False, parent=self, name=f"Retrograde{add_pitch}")
 
     @once_per_arg
     def Retrograde_without_rhyme(self, add_pitch: int = 0) -> PitchSegment:
         """
-        This function creates a Retrograde transformation of self without changing the rhythm.
+        This function creates a Retrograde transformation of self without changing the pitch_class_series.
         :param add_pitch: Transposition num.
-        :return: Retrograded new PitchSegment object.
+        :return: Retrograded new PitchSegment object_.
         """
-        new_pitch_set = list(reversed(self.pitch_set))[:]
+        new_pitch_set = list(reversed(self.pitch_series))[:]
         if add_pitch == 0:
-            return series.PitchSegment([new_pitch_set, self.duration_set[:]],
-                                       new_tree=self, parent=self, name="Retrograde without rhyme")
+            return PitchSegment([new_pitch_set, self.rhythm[:]],
+                                new_tree=False, parent=self, name="Retrograde without pitch_class_series")
         new_pitch_set = [new_pitch + int(add_pitch) for new_pitch in new_pitch_set]
-        return series.PitchSegment([new_pitch_set, self.duration_set[:]],
-                                   new_tree=self, parent=self, name=f"Retrograde{add_pitch}")
+        return PitchSegment([new_pitch_set, self.rhythm[:]],
+                            new_tree=False, parent=self, name=f"Retrograde{add_pitch}")
 
     @once_per_arg
     def Inversion(self, axes: int) -> PitchSegment:
         """
-        This function creates an Inversion transformation of self without changing the rhythm.
+        This function creates an Inversion transformation of self without changing the pitch_class_series.
         :param axes: An int to invert each pitch in the set.
-        :return: Inverted new PitchSegment object.
+        :return: Inverted new PitchSegment object_.
         """
-        new_pitch_set = [2 * axes - pitch for pitch in self.pitch_set]
-        return series.PitchSegment([new_pitch_set, self.duration_set[:]],
-                                   new_tree=self, parent=self, name=f"Inversion{axes}")
+        new_pitch_set = [2 * axes - pitch for pitch in self.pitch_series]
+        return PitchSegment([new_pitch_set, self.rhythm[:]],
+                            new_tree=False, parent=self, name=f"Inversion{axes}")
 
     @once_per_arg
     def RetrogradeInversion(self, axes: int) -> PitchSegment:
         """
-        This function creates a Retrograde then Inversion transformation of self with changed rhythm.
+        This function creates a Retrograde then Inversion transformation of self with changed pitch_class_series.
         :param axes: An int to invert each pitch in the set.
-        :return: Retrograde then Inversion new PitchSegment object.
+        :return: Retrograde then Inversion new PitchSegment object_.
         """
-        new_pitch_set = reversed([2 * axes - pitch for pitch in self.pitch_set])
-        new_duration_set = reversed(self.duration_set)
-        return series.PitchSegment([new_pitch_set, new_duration_set],
-                                   new_tree=self, parent=self, name=f"RetrogradeInversion{axes} (with rhyme)")
+        new_pitch_set = reversed([2 * axes - pitch for pitch in self.pitch_series])
+        new_duration_set = reversed(self.rhythm)
+        return PitchSegment([new_pitch_set, new_duration_set],
+                            new_tree=False, parent=self, name=f"RetrogradeInversion{axes} (with pitch_class_series)")
 
     @once_per_arg
     def Rotation_without_rhyme(self, num: int, add_pitch: int = 0) -> PitchSegment:
         """
-        This function creates a Rotation transformation of self without changing the rhythm.
+        This function creates a Rotation transformation of self without changing the pitch_class_series.
         :param num: Rotation num
         :param add_pitch: Transposition num.
-        :return: Roted new PitchSegment object.
+        :return: Roted new PitchSegment object_.
         """
         if not 0 <= num < self.length:
             raise ValueError("The attribute 'num' should be smaller than length of the series.")
-        new_pitch_set = [self.pitch_set[(ii + num) % self.length] for ii in range(self.length)]
+        new_pitch_set = [self.pitch_series[(ii + num) % self.length] for ii in range(self.length)]
         if add_pitch == 0:
-            return series.PitchSegment([new_pitch_set[:], self.duration_set[:]],
-                                       new_tree=self, parent=self, name=f"Rotation{num} (without rhyme)")
+            return PitchSegment([new_pitch_set[:], self.rhythm[:]],
+                                new_tree=False, parent=self, name=f"Rotation{num} (without pitch_class_series)")
         new_pitch_set = [new_pitch + int(add_pitch) for new_pitch in new_pitch_set]
-        return series.PitchSegment([new_pitch_set[:], self.duration_set[:]],
-                                   new_tree=self, parent=self, name=f"Rotation{num} (without rhyme),T{add_pitch}")
+        return PitchSegment([new_pitch_set[:], self.rhythm[:]],
+                            new_tree=False, parent=self, name=f"Rotation{num} (without pitch_class_series),T{add_pitch}")
 
     @once_per_arg
     def Rotation_with_rhyme(self, num: int, add_pitch: int = 0) -> PitchSegment:
         """
-        This function creates a Rotation transformation of self with changed rhythm.
+        This function creates a Rotation transformation of self with changed pitch_class_series.
         :param num: Rotation num
         :param add_pitch: Transposition num.
-        :return: Retrograded new PitchSegment object.
+        :return: Retrograded new PitchSegment object_.
         """
         if not 0 <= num < self.length:
             raise ValueError("The attribute 'num' should be smaller than length of the series.")
-        new_pitch_set = [self.pitch_set[(ii + num) % self.length] for ii in range(self.length)]
-        new_duration_set = [self.duration_set[(ii + num) % self.length] for ii in range(self.length)]
+        new_pitch_set = [self.pitch_series[(ii + num) % self.length] for ii in range(self.length)]
+        new_duration_set = [self.rhythm[(ii + num) % self.length] for ii in range(self.length)]
         if add_pitch == 0:
-            return series.PitchSegment([new_pitch_set[:], new_duration_set[:]],
-                                       new_tree=self, parent=self, name=f"Rotation{num} (with rhyme)")
+            return PitchSegment([new_pitch_set[:], new_duration_set[:]],
+                                new_tree=False, parent=self, name=f"Rotation{num} (with pitch_class_series)")
         new_pitch_set = [new_pitch + int(add_pitch) for new_pitch in new_pitch_set]
-        return series.PitchSegment([new_pitch_set[:], new_duration_set[:]],
-                                   new_tree=self, parent=self, name=f"Rotation{num} (with rhyme),T{add_pitch}")
+        return PitchSegment([new_pitch_set[:], new_duration_set[:]],
+                            new_tree=False, parent=self, name=f"Rotation{num} (with pitch_class_series),T{add_pitch}")
 
     def play(self, pg_player=None, bpm=80, instrument='piano'):
         """
         :param pg_player: Pygame.midi.Output(int) var. If you haven't set it, keep it None.
         eg:
         player = pygame.midi.output(0)
         ps1.play(pg_player=player)
@@ -273,141 +550,11 @@
         :param instrument: instrument.
         """
         from .._player import play_pitch_segment
         play_pitch_segment(pg_player, self, instrument=instrument, bpm=bpm)
         del play_pitch_segment
 
 
-class PitchClassSegment(PitchSegment):
-    def __init__(self, segment, __style=None):
-        """ Variable 'series' should be a list of two lists.   """
-        super().__init__(segment, __style=None)
-        self.pitch_class_set = self.pitch_set
-        self.pitch_tend = None
-        self.rhythm_intensity_tend = None
-
-    def __hash__(self):
-        return hash(self.segment)
-
-    def __eq__(self, other):
-        return self.segment == other.segment
-
-    def __iter__(self):
-        return iter(zip(self.pitch_class_set, self.duration_set))
-
-    def __add__(self, add_pitch):
-        new_pitch_class_set = [new_pitch + int(add_pitch) for new_pitch in self.pitch_class_set]
-        return PitchClassSegment([new_pitch_class_set, self.duration_set][:]), self, f"Transposition{add_pitch}"
-
-    def __sub__(self, sub_pitch):
-        new_pitch_class_set = [new_pitch - int(sub_pitch) for new_pitch in self.pitch_class_set]
-        return PitchClassSegment([new_pitch_class_set, self.duration_set][:]), self, f"Transposition{12 - sub_pitch}"
-
-    def __mod__(self, number):
-        raise RuntimeError("")
-
-    def __getitem__(self, item):
-        return self.pitch_class_set[int(item)], self.duration_set[int(item)]
-
-    def __setitem__(self, key, value):
-        """
-        Variable *keys includes two element.
-        Variable "values" is two-element list.
-        """
-        new_pc_set = self.pitch_set
-        new_pc_set[key] = value
-        return PitchClassSegment(
-            [new_pc_set, self.duration_set[:]]), self, f"Reset pitch set[{key}]{note_value[value]}"
-
-    @once_per_arg
-    def __reversed__(self):
-        new_pc_set = reversed(self.pitch_set)[:]
-        new_duration_set = reversed(self.duration_set)[:]
-        return PitchClassSegment([new_pc_set, new_duration_set]), self, "Retrograde (with rhyme)"
-
-    @once_per_arg
-    def new_segment(self, note_num, total_duration, first_note, note_scale, style):
-        """ To generate a new series while original series is empty.  """
-        if self.segment:
-            raise RuntimeError("The function 'new_segment' is only used for empty pitch series.")
-        _segment = basicGenerator.randomSegment(note_num, total_duration, first_note, note_scale, style)
-        self.__init__(_segment, __style=style)
-
-    @once_per_arg
-    def change_rhyme(self, total_duration, new_style):
-        """ To overwrite a new rhyme to the pitch set.   """
-        self.style = new_style
-        _segment = [self.pitch_set, basicGenerator.randomRhythm(self.length, total_duration, new_style)]
-        return PitchClassSegment(_segment), self, "Different rhyme"
-
-    def get_average(self):
-        return self.w_average
-
-    def get_pitch_tend(self):
-        return self.pitch_tend
-
-    def get_rhythm_intensity_tend(self):
-        return self.rhythm_intensity_tend
-
-    @once_per_arg
-    def Transposition(self, add_pitch):
-        new_pitch_set = [new_pitch + int(add_pitch) for new_pitch in self.pitch_set]
-        return PitchClassSegment([new_pitch_set, self.duration_set][:]), self, f"Transposition{add_pitch}"
-
-    @once_per_arg
-    def Retrograde_with_rhyme(self, add_pitch=0):
-        new_pitch_set = reversed(self.pitch_set)[:]
-        new_duration_set = reversed(self.duration_set)[:]
-        if add_pitch == 0:
-            return PitchClassSegment([new_pitch_set, new_duration_set]), self, "Retrograde with rhyme"
-        new_pitch_set = [new_pitch + int(add_pitch) for new_pitch in new_pitch_set]
-        return PitchClassSegment([new_pitch_set, new_duration_set]), self, f"Retrograde{add_pitch}"
-
-    @once_per_arg
-    def Retrograde_without_rhyme(self, add_pitch=0):
-        new_pitch_set = reversed(self.pitch_set)[:]
-        if add_pitch == 0:
-            return PitchClassSegment([new_pitch_set, self.duration_set[:]]), self, "Retrograde without rhyme"
-        new_pitch_set = [new_pitch + int(add_pitch) for new_pitch in new_pitch_set]
-        return PitchClassSegment([new_pitch_set, self.duration_set[:]]), self, "Retrograde" + str(add_pitch)
-
-    @once_per_arg
-    def Inversion(self, axes):
-        new_pitch_set = [2 * int(axes) - pitch for pitch in self.pitch_set]
-        return PitchClassSegment([new_pitch_set, self.duration_set[:]]), self, "Inversion" + str(axes)
-
-    @once_per_arg
-    def RetrogradeInversion(self, axes):
-        new_pitch_set = reversed([2 * int(axes) - pitch for pitch in self.pitch_set])
-        new_duration_set = reversed(self.duration_set)
-        return PitchClassSegment([new_pitch_set, new_duration_set]), self, "Retrograde Inversion" + str(axes)
-
-    @once_per_arg
-    def Rotation_without_rhyme(self, num, add_pitch=0):
-        if not 0 <= num < self.length:
-            raise ValueError("The attribute 'num' should be smaller than length of the series.")
-        new_pitch_set = [self.pitch_set[(ii + num) % self.length] for ii in range(self.length)]
-        if add_pitch == 0:
-            return PitchClassSegment([new_pitch_set[:], self.duration_set[:]]
-                                     ), self, f"Rotation{num} (without rhyme)"
-        new_pitch_set = [new_pitch + int(add_pitch) for new_pitch in new_pitch_set]
-        return PitchClassSegment([new_pitch_set[:], self.duration_set[:]]
-                                 ), self, f"Rotation{num} (without rhyme),T{add_pitch}"
-
-    @once_per_arg
-    def Rotation_with_rhyme(self, num, add_pitch=0):
-        if not 0 <= num < self.length:
-            raise ValueError("The attribute 'num' should be smaller than length of the series.")
-        new_pitch_set = [self.pitch_set[(ii + num) % self.length] for ii in range(self.length)]
-        new_duration_set = [self.duration_set[(ii + num) % self.length] for ii in range(self.length)]
-        if add_pitch == 0:
-            return PitchClassSegment(
-                [new_pitch_set[:], new_duration_set[:]]), self, f"Rotation{num} (with rhyme)"
-        new_pitch_set = [new_pitch + int(add_pitch) for new_pitch in new_pitch_set]
-        return PitchClassSegment(
-            [new_pitch_set[:], new_duration_set[:]]), self, f"Rotation{num} (with rhyme),T{add_pitch}"
-
-
 # TODO: 轮廓截段
 class ContourSegment:
     def __init__(self, segment):
         self.pitch_set = segment[0]
```

### Comparing `pypcs-0.0.1/setup.py` & `pypcs-0.0.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import setuptools
 
 
-VERSION = 1
+VERSION = 3
 
 
 setuptools.setup(
     name="pypcs",
     version='0.0.' + str(VERSION),
     author="Jason Lee",
     author_email="2593292614@qq.com",
     description="",
     long_description=open('README.md', 'r', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
-    url="https://github.com",
+    install_package_data=True,
+    url="https://github.com/JasonLee-p/pyPCS",
     install_requires=[
         'numpy==1.24.2',
-        'pygame==2.3.0'
+        'pygame==2.3.0',
+        'rtmidi==2.5.0',
+        'webcolors==1.12',
+        'Pillow==9.5.0'
     ],
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
         "Operating System :: OS Independent",
     ],
```

