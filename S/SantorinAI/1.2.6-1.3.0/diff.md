# Comparing `tmp/SantorinAI-1.2.6.tar.gz` & `tmp/SantorinAI-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SantorinAI-1.2.6.tar", last modified: Mon May 15 07:26:41 2023, max compression
+gzip compressed data, was "SantorinAI-1.3.0.tar", last modified: Wed May 17 20:12:41 2023, max compression
```

## Comparing `SantorinAI-1.2.6.tar` & `SantorinAI-1.3.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:26:41.389600 SantorinAI-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-15 07:26:41.389600 SantorinAI-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:26:41.389600 SantorinAI-1.2.6/SantorinAI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-15 07:26:41.000000 SantorinAI-1.2.6/SantorinAI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-15 07:26:41.000000 SantorinAI-1.2.6/SantorinAI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 07:26:41.000000 SantorinAI-1.2.6/SantorinAI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 07:26:41.000000 SantorinAI-1.2.6/SantorinAI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 07:26:41.000000 SantorinAI-1.2.6/SantorinAI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:26:41.389600 SantorinAI-1.2.6/santorinai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/santorinai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/santorinai/board.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:26:41.389600 SantorinAI-1.2.6/santorinai/board_displayer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/santorinai/board_displayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/santorinai/board_displayer/board_displayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/santorinai/pawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/santorinai/player.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:26:41.389600 SantorinAI-1.2.6/santorinai/player_examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/santorinai/player_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/santorinai/player_examples/first_choice_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/santorinai/player_examples/random_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/santorinai/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 07:26:41.389600 SantorinAI-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:26:41.389600 SantorinAI-1.2.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/test/test_board.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/test/test_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:12:41.983763 SantorinAI-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-17 20:12:41.983763 SantorinAI-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:12:41.979763 SantorinAI-1.3.0/SantorinAI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-17 20:12:41.000000 SantorinAI-1.3.0/SantorinAI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-17 20:12:41.000000 SantorinAI-1.3.0/SantorinAI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 20:12:41.000000 SantorinAI-1.3.0/SantorinAI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 20:12:41.000000 SantorinAI-1.3.0/SantorinAI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 20:12:41.000000 SantorinAI-1.3.0/SantorinAI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:12:41.979763 SantorinAI-1.3.0/santorinai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:12:41.979763 SantorinAI-1.3.0/santorinai/board_displayer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/board_displayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/board_displayer/board_displayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/pawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/player.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:12:41.983763 SantorinAI-1.3.0/santorinai/player_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/player_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/player_examples/basic_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/player_examples/first_choice_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/player_examples/random_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 20:12:41.983763 SantorinAI-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:12:41.983763 SantorinAI-1.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/test/test_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/test/test_tester.py
```

### Comparing `SantorinAI-1.2.6/LICENSE` & `SantorinAI-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.6/PKG-INFO` & `SantorinAI-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.2.6
+Version: 1.3.0
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `SantorinAI-1.2.6/README.md` & `SantorinAI-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.6/SantorinAI.egg-info/PKG-INFO` & `SantorinAI-1.3.0/SantorinAI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.2.6
+Version: 1.3.0
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `SantorinAI-1.2.6/SantorinAI.egg-info/SOURCES.txt` & `SantorinAI-1.3.0/SantorinAI.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,12 +10,13 @@
 santorinai/board.py
 santorinai/pawn.py
 santorinai/player.py
 santorinai/tester.py
 santorinai/board_displayer/__init__.py
 santorinai/board_displayer/board_displayer.py
 santorinai/player_examples/__init__.py
+santorinai/player_examples/basic_player.py
 santorinai/player_examples/first_choice_player.py
 santorinai/player_examples/random_player.py
 test/__init__.py
 test/test_board.py
 test/test_tester.py
```

### Comparing `SantorinAI-1.2.6/santorinai/board.py` & `SantorinAI-1.3.0/santorinai/board.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.6/santorinai/board_displayer/board_displayer.py` & `SantorinAI-1.3.0/santorinai/board_displayer/board_displayer.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.6/santorinai/pawn.py` & `SantorinAI-1.3.0/santorinai/pawn.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.6/santorinai/player.py` & `SantorinAI-1.3.0/santorinai/player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.6/santorinai/player_examples/first_choice_player.py` & `SantorinAI-1.3.0/santorinai/player_examples/first_choice_player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.6/santorinai/player_examples/random_player.py` & `SantorinAI-1.3.0/santorinai/player_examples/random_player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.6/santorinai/tester.py` & `SantorinAI-1.3.0/santorinai/tester.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class Tester:
     """
     Run the games with SantorinAI playes, do statistics display the results
     """
 
     verbose_level = 2
     delay_between_moves = 0
-    display_board = True
+    display_board = False
 
     def display_message(self, message, verbose_level=1):
         """
         Display a message if verbose is True
 
         Args:
             message (str): the message to display
@@ -144,7 +144,12 @@
             + "%)"
         )
         print(
             f"Player {players[1].name()} won {nb_victories[1]} times ("
             + str(round(nb_victories[1] / nb_games * 100, 2))
             + "%)"
         )
+
+        return {
+            players[0].name(): nb_victories[0],
+            players[1].name(): nb_victories[1],
+        }
```

### Comparing `SantorinAI-1.2.6/setup.py` & `SantorinAI-1.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="SantorinAI",
-    version="1.2.6",
+    version="1.3.0",
     author="Tom Mansion",
     author_email="tomansion@yahoo.fr",
     description="A Python library for the Santorini board game",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tomansion/santorinai",
     packages=find_packages(),
```

### Comparing `SantorinAI-1.2.6/test/test_board.py` & `SantorinAI-1.3.0/test/test_board.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.6/test/test_tester.py` & `SantorinAI-1.3.0/test/test_tester.py`

 * *Files identical despite different names*

