# Comparing `tmp/pyloggor-1.1.1.tar.gz` & `tmp/pyloggor-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloggor-1.1.1.tar", last modified: Thu Mar  9 07:32:53 2023, max compression
+gzip compressed data, was "pyloggor-1.1.2.tar", last modified: Wed May 17 12:49:21 2023, max compression
```

## Comparing `pyloggor-1.1.1.tar` & `pyloggor-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-09 07:32:53.984735 pyloggor-1.1.1/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2022-10-29 03:33:26.000000 pyloggor-1.1.1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     6226 2023-03-09 07:32:53.984152 pyloggor-1.1.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5673 2022-10-13 14:54:07.000000 pyloggor-1.1.1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-09 07:32:53.979172 pyloggor-1.1.1/pyloggor/
--rwxrwxrwx   0 root         (0) root         (0)       31 2022-10-29 03:33:26.000000 pyloggor-1.1.1/pyloggor/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6082 2023-03-09 07:32:14.000000 pyloggor-1.1.1/pyloggor/pyloggor.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-09 07:32:53.982994 pyloggor-1.1.1/pyloggor.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     6226 2023-03-09 07:32:53.000000 pyloggor-1.1.1/pyloggor.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      196 2023-03-09 07:32:53.000000 pyloggor-1.1.1/pyloggor.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-03-09 07:32:53.000000 pyloggor-1.1.1/pyloggor.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        9 2023-03-09 07:32:53.000000 pyloggor-1.1.1/pyloggor.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-03-09 07:32:53.984931 pyloggor-1.1.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      701 2023-03-09 07:29:54.000000 pyloggor-1.1.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 12:49:21.351281 pyloggor-1.1.2/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-09 10:25:32.000000 pyloggor-1.1.2/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     6134 2023-05-17 12:49:21.350807 pyloggor-1.1.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5673 2023-05-09 10:25:30.000000 pyloggor-1.1.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 12:49:21.346703 pyloggor-1.1.2/pyloggor/
+-rwxrwxrwx   0 root         (0) root         (0)       31 2023-05-09 10:25:30.000000 pyloggor-1.1.2/pyloggor/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6790 2023-05-17 12:47:27.000000 pyloggor-1.1.2/pyloggor/pyloggor.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 12:49:21.349962 pyloggor-1.1.2/pyloggor.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     6134 2023-05-17 12:49:21.000000 pyloggor-1.1.2/pyloggor.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      227 2023-05-17 12:49:21.000000 pyloggor-1.1.2/pyloggor.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-17 12:49:21.000000 pyloggor-1.1.2/pyloggor.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        5 2023-05-17 12:49:21.000000 pyloggor-1.1.2/pyloggor.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        9 2023-05-17 12:49:21.000000 pyloggor-1.1.2/pyloggor.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-17 12:49:21.351432 pyloggor-1.1.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      640 2023-05-17 12:48:54.000000 pyloggor-1.1.2/setup.py
```

### Comparing `pyloggor-1.1.1/LICENSE` & `pyloggor-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyloggor-1.1.1/PKG-INFO` & `pyloggor-1.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pyloggor
-Version: 1.1.1
+Version: 1.1.2
 Summary: An incredibly versatile yet simple logging system.
 Home-page: https://www.github.com/PrivatePandaCO/pyloggor
 Author: Parth Mittal
 Author-email: parth@privatepanda.co
 License: MIT
 Project-URL: Documentation, https://github.com/PrivatePandaCO/pyloggor/blob/master/README.md
 Project-URL: Github, https://github.com/PrivatePandaCO/pyloggor
-Project-URL: Changelog, https://github.com/PrivatePandaCO/pyloggor/blob/master/Changelog.md
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 The easiest and perhaps the most versatile logger for python, in hundred lines.
 
 ## Table of Contents
 - [Installation](#Installation)
```

### Comparing `pyloggor-1.1.1/README.md` & `pyloggor-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyloggor-1.1.1/pyloggor/pyloggor.py` & `pyloggor-1.1.2/pyloggor/pyloggor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,54 @@
+import inspect
 import os
+import threading
+import time
 from datetime import datetime
 from typing import Literal, Optional
-import time
+
+import pytz
 
 
 class FileHandler:
-    def __init__(self, fn):
+    def __init__(self, fn, log_freq):
+        self.log_freq = log_freq
         self.fn = fn
+        self.cache = []
         open(fn, "w") if not os.path.exists(fn) else ...
+        threading.Thread(target=self._log, daemon=True).start()
 
     def write(self, msg):
-        with open(self.fn, "a") as f:
-            f.write(f"{msg}\n")
+        self.cache.append(msg)
+
+    def _log(self):
+        while True:
+            if self.cache:
+                f = open(self.fn, "a")
+                f.write("\n".join(self.cache) + "\n")
+                f.close()
+            time.sleep(self.log_freq)
 
 
 class pyloggor:
     default_level_colours = {
         "DEBUG": "\033[1;36m",
         "INFO": "\033[1;32m",
         "WARNING": "\033[1;33m",
         "ERROR": "\033[1;31m",
         "CRITICAL": "\033[1;35m",
     }
 
+    default_level_symbols = {
+        "DEBUG": "D",
+        "INFO": "I",
+        "WARNING": "W",
+        "ERROR": "E",
+        "CRITICAL": "C",
+    }
+
     def __init__(
         self,
         *,
         file_output_level: Literal["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"] = "DEBUG",
         console_output_level: Literal["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"] = "DEBUG",
         topic_adjustment_space: int = 15,
         file_adjustment_space: int = 15,
@@ -36,28 +58,24 @@
         file_align: Literal["left", "center", "centre", "right"] = "left",
         fn=False,
         console_output=True,
         level_colours: dict = default_level_colours,
         default_colour="\033[1;37m",
         delim="|",
         datefmt=r"%d-%b-%y, %H:%M:%S:%f",
-        level_symbols={
-            "DEBUG": "D",
-            "INFO": "I",
-            "WARNING": "W",
-            "ERROR": "E",
-            "CRITICAL": "C",
-        },
+        level_symbols=default_level_symbols,
+        auto_filename=True,
         show_file=True,
         show_symbol=True,
         show_time=True,
         show_topic=True,
         title_level=False,
+        file_log_freq=3,
     ):
-        self.file = FileHandler(fn) if fn else False
+        self.file = FileHandler(fn, file_log_freq) if fn else False
         self.file_output_level = file_output_level if self.file else "NOLOG"
         self.console_output_level = console_output_level
         self.topic_adjustment_space = topic_adjustment_space
         self.file_adjustment_space = file_adjustment_space
         self.level_adjustment_space = level_adjustment_space
         self.center_level = level_align
         self.center_file = file_align
@@ -66,14 +84,15 @@
         self.level_symbols = level_symbols
 
         self.level_colours = level_colours
         self.default_colour = default_colour
         self.delim = delim
         self.datefmt = datefmt
 
+        self.auto_filename = auto_filename
         self.show_file = show_file
         self.show_symbol = show_symbol
         self.show_time = show_time
         self.show_topic = show_topic
         self.title_level = title_level
 
         self.default_levels = {
@@ -110,15 +129,15 @@
         msg="NoMessage",  # I don't know why people do this
         extras: Optional[dict] = None,
         console_output: bool = None,
         file_output: bool = None,
     ):
         level = level.title() if self.title_level else level.upper()
 
-        time_str = datetime.fromtimestamp(time.time()).strftime(self.datefmt)
+        time_str = datetime.fromtimestamp(time.time(), tz=pytz.UTC).strftime(self.datefmt)
 
         if extras:
             extras_str = f"{self.delim} {self.extras_builder(extras)}"
         else:
             extras_str = ""
 
         if level in self.level_symbols.keys():
@@ -130,14 +149,17 @@
         if self.show_symbol:
             _msg += f"[{level_symbol}] "
 
         if self.show_time:
             _msg += f"{time_str} {self.delim} "
         _msg += f"{self.beautify(level, self.level_adjustment_space, self.center_level)} {self.delim} "
         if self.show_file:
+            if self.auto_filename:
+                frame = inspect.currentframe().f_back
+                file = f"{os.path.relpath(frame.f_code.co_filename, start=os.getcwd())}:{frame.f_lineno}"
             _msg += f"{self.beautify(file, self.file_adjustment_space, self.center_file)} {self.delim} "
         if self.show_topic:
             _msg += f"{self.beautify(topic, self.topic_adjustment_space, self.center_topic)} {self.delim} "
         _msg += f"{msg} {extras_str}"
 
         if level.upper() in self.level_colours.keys():
             level_colour = self.level_colours[level.upper()]
```

### Comparing `pyloggor-1.1.1/pyloggor.egg-info/PKG-INFO` & `pyloggor-1.1.2/pyloggor.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pyloggor
-Version: 1.1.1
+Version: 1.1.2
 Summary: An incredibly versatile yet simple logging system.
 Home-page: https://www.github.com/PrivatePandaCO/pyloggor
 Author: Parth Mittal
 Author-email: parth@privatepanda.co
 License: MIT
 Project-URL: Documentation, https://github.com/PrivatePandaCO/pyloggor/blob/master/README.md
 Project-URL: Github, https://github.com/PrivatePandaCO/pyloggor
-Project-URL: Changelog, https://github.com/PrivatePandaCO/pyloggor/blob/master/Changelog.md
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 The easiest and perhaps the most versatile logger for python, in hundred lines.
 
 ## Table of Contents
 - [Installation](#Installation)
```

### Comparing `pyloggor-1.1.1/setup.py` & `pyloggor-1.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
     name="pyloggor",
-    version="1.1.1",
+    version="1.1.2",
     description="An incredibly versatile yet simple logging system.",
     author="Parth Mittal",
     author_email="parth@privatepanda.co",
     url="https://www.github.com/PrivatePandaCO/pyloggor",
     license="MIT",
     packages=["pyloggor"],
+    install_requires=["pytz"],
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     project_urls={
         "Documentation": "https://github.com/PrivatePandaCO/pyloggor/blob/master/README.md",
         "Github": "https://github.com/PrivatePandaCO/pyloggor",
-        "Changelog": "https://github.com/PrivatePandaCO/pyloggor/blob/master/Changelog.md",
     },
 )
```

