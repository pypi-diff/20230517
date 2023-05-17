# Comparing `tmp/pynterface-0.0.3.tar.gz` & `tmp/pynterface-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynterface-0.0.3.tar", last modified: Mon May 15 15:05:34 2023, max compression
+gzip compressed data, was "pynterface-0.0.4.tar", last modified: Wed May 17 03:19:17 2023, max compression
```

## Comparing `pynterface-0.0.3.tar` & `pynterface-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-15 15:05:34.769913 pynterface-0.0.3/
--rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-05-04 02:59:32.000000 pynterface-0.0.3/LICENSE
--rw-r--r--   0 vivaan     (501) staff       (20)       33 2023-05-14 03:48:17.000000 pynterface-0.0.3/MANIFEST.in
--rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-05-15 15:05:34.769599 pynterface-0.0.3/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)     1156 2023-05-14 04:10:04.000000 pynterface-0.0.3/README.md
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-15 15:05:34.768143 pynterface-0.0.3/pynterface/
--rw-r--r--   0 vivaan     (501) staff       (20)      238 2023-05-15 15:05:09.000000 pynterface-0.0.3/pynterface/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     2840 2023-05-14 01:50:32.000000 pynterface-0.0.3/pynterface/input.py
--rw-r--r--   0 vivaan     (501) staff       (20)     6495 2023-05-09 23:26:51.000000 pynterface-0.0.3/pynterface/loading.py
--rw-r--r--   0 vivaan     (501) staff       (20)     3367 2023-05-15 15:05:04.000000 pynterface-0.0.3/pynterface/menu.py
--rw-r--r--   0 vivaan     (501) staff       (20)     5444 2023-05-14 18:25:39.000000 pynterface-0.0.3/pynterface/printing.py
--rw-r--r--   0 vivaan     (501) staff       (20)     5848 2023-05-15 14:51:42.000000 pynterface-0.0.3/pynterface/style.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-15 15:05:34.769242 pynterface-0.0.3/pynterface.egg-info/
--rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-05-15 15:05:34.000000 pynterface-0.0.3/pynterface.egg-info/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)      301 2023-05-15 15:05:34.000000 pynterface-0.0.3/pynterface.egg-info/SOURCES.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-15 15:05:34.000000 pynterface-0.0.3/pynterface.egg-info/dependency_links.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       11 2023-05-15 15:05:34.000000 pynterface-0.0.3/pynterface.egg-info/top_level.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-15 15:05:34.770001 pynterface-0.0.3/setup.cfg
--rw-r--r--   0 vivaan     (501) staff       (20)      612 2023-05-14 04:04:56.000000 pynterface-0.0.3/setup.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-17 03:19:17.858839 pynterface-0.0.4/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-05-04 02:59:32.000000 pynterface-0.0.4/LICENSE
+-rw-r--r--   0 vivaan     (501) staff       (20)       33 2023-05-14 03:48:17.000000 pynterface-0.0.4/MANIFEST.in
+-rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-05-17 03:19:17.858522 pynterface-0.0.4/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)     1156 2023-05-14 04:10:04.000000 pynterface-0.0.4/README.md
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-17 03:19:17.856767 pynterface-0.0.4/pynterface/
+-rw-r--r--   0 vivaan     (501) staff       (20)      238 2023-05-17 03:18:45.000000 pynterface-0.0.4/pynterface/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     2840 2023-05-15 19:24:45.000000 pynterface-0.0.4/pynterface/input.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     6541 2023-05-17 03:18:29.000000 pynterface-0.0.4/pynterface/loading.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     3367 2023-05-15 15:05:04.000000 pynterface-0.0.4/pynterface/menu.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     5444 2023-05-14 18:25:39.000000 pynterface-0.0.4/pynterface/printing.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     5848 2023-05-15 14:51:42.000000 pynterface-0.0.4/pynterface/style.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-17 03:19:17.858119 pynterface-0.0.4/pynterface.egg-info/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-05-17 03:19:17.000000 pynterface-0.0.4/pynterface.egg-info/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)      301 2023-05-17 03:19:17.000000 pynterface-0.0.4/pynterface.egg-info/SOURCES.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-17 03:19:17.000000 pynterface-0.0.4/pynterface.egg-info/dependency_links.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       11 2023-05-17 03:19:17.000000 pynterface-0.0.4/pynterface.egg-info/top_level.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-17 03:19:17.858932 pynterface-0.0.4/setup.cfg
+-rw-r--r--   0 vivaan     (501) staff       (20)      612 2023-05-14 04:04:56.000000 pynterface-0.0.4/setup.py
```

### Comparing `pynterface-0.0.3/LICENSE` & `pynterface-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.3/PKG-INFO` & `pynterface-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynterface
-Version: 0.0.3
+Version: 0.0.4
 Summary: Terminal-Based Printing Tools!
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://pynterface.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pynterface-0.0.3/README.md` & `pynterface-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.3/pynterface/input.py` & `pynterface-0.0.4/pynterface/input.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.3/pynterface/loading.py` & `pynterface-0.0.4/pynterface/loading.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Supports loading animations, inspired by Auto-GPT's spinner class, found here: https://github.com/Significant-Gravitas/Auto-GPT/blob/master/autogpt/spinner.py
 This version supports customizable cycling as well as default classes for quick access. You can also print messages above the spinner.
 """
 from __future__ import annotations
 from threading import Thread
 from time import sleep
+from sys import stdout
 
 class Loader():
     
     def __init__(self, message: str, cycle: list[str], delay: int, hide_cursor: bool = True) -> None:
 
         """
         Creates a new Loader with a message which appears on the same line as the cycler.
@@ -78,14 +79,15 @@
     def __display(self, item):
         """
         Clears and displays the message.
         """
         self.__clear_animated()
         self.prev_length = len(item)
         print("\r" + self.message + item, end="")
+        stdout.flush()
 
     def __enter__(self) -> Loader:
         self.runner = Thread(target=self.__run)
         self.runner.start()
         return self
 
     def __exit__(self, _, __, ___):
```

### Comparing `pynterface-0.0.3/pynterface/menu.py` & `pynterface-0.0.4/pynterface/menu.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.3/pynterface/printing.py` & `pynterface-0.0.4/pynterface/printing.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.3/pynterface/style.py` & `pynterface-0.0.4/pynterface/style.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.3/pynterface.egg-info/PKG-INFO` & `pynterface-0.0.4/pynterface.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynterface
-Version: 0.0.3
+Version: 0.0.4
 Summary: Terminal-Based Printing Tools!
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://pynterface.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pynterface-0.0.3/setup.py` & `pynterface-0.0.4/setup.py`

 * *Files identical despite different names*

