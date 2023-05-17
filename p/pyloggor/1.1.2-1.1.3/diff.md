# Comparing `tmp/pyloggor-1.1.2.tar.gz` & `tmp/pyloggor-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloggor-1.1.2.tar", last modified: Wed May 17 12:49:21 2023, max compression
+gzip compressed data, was "pyloggor-1.1.3.tar", last modified: Wed May 17 17:28:43 2023, max compression
```

## Comparing `pyloggor-1.1.2.tar` & `pyloggor-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 12:49:21.351281 pyloggor-1.1.2/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-09 10:25:32.000000 pyloggor-1.1.2/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     6134 2023-05-17 12:49:21.350807 pyloggor-1.1.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5673 2023-05-09 10:25:30.000000 pyloggor-1.1.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 12:49:21.346703 pyloggor-1.1.2/pyloggor/
--rwxrwxrwx   0 root         (0) root         (0)       31 2023-05-09 10:25:30.000000 pyloggor-1.1.2/pyloggor/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6790 2023-05-17 12:47:27.000000 pyloggor-1.1.2/pyloggor/pyloggor.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 12:49:21.349962 pyloggor-1.1.2/pyloggor.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     6134 2023-05-17 12:49:21.000000 pyloggor-1.1.2/pyloggor.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      227 2023-05-17 12:49:21.000000 pyloggor-1.1.2/pyloggor.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-17 12:49:21.000000 pyloggor-1.1.2/pyloggor.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        5 2023-05-17 12:49:21.000000 pyloggor-1.1.2/pyloggor.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        9 2023-05-17 12:49:21.000000 pyloggor-1.1.2/pyloggor.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-17 12:49:21.351432 pyloggor-1.1.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      640 2023-05-17 12:48:54.000000 pyloggor-1.1.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 17:28:43.310967 pyloggor-1.1.3/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-09 10:25:32.000000 pyloggor-1.1.3/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     6134 2023-05-17 17:28:43.310464 pyloggor-1.1.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5673 2023-05-09 10:25:30.000000 pyloggor-1.1.3/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 17:28:43.305507 pyloggor-1.1.3/pyloggor/
+-rwxrwxrwx   0 root         (0) root         (0)       31 2023-05-09 10:25:30.000000 pyloggor-1.1.3/pyloggor/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7431 2023-05-17 17:27:06.000000 pyloggor-1.1.3/pyloggor/pyloggor.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 17:28:43.309523 pyloggor-1.1.3/pyloggor.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     6134 2023-05-17 17:28:43.000000 pyloggor-1.1.3/pyloggor.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      227 2023-05-17 17:28:43.000000 pyloggor-1.1.3/pyloggor.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-17 17:28:43.000000 pyloggor-1.1.3/pyloggor.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        5 2023-05-17 17:28:43.000000 pyloggor-1.1.3/pyloggor.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        9 2023-05-17 17:28:43.000000 pyloggor-1.1.3/pyloggor.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-17 17:28:43.311121 pyloggor-1.1.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      640 2023-05-17 17:27:59.000000 pyloggor-1.1.3/setup.py
```

### Comparing `pyloggor-1.1.2/LICENSE` & `pyloggor-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyloggor-1.1.2/PKG-INFO` & `pyloggor-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyloggor
-Version: 1.1.2
+Version: 1.1.3
 Summary: An incredibly versatile yet simple logging system.
 Home-page: https://www.github.com/PrivatePandaCO/pyloggor
 Author: Parth Mittal
 Author-email: parth@privatepanda.co
 License: MIT
 Project-URL: Documentation, https://github.com/PrivatePandaCO/pyloggor/blob/master/README.md
 Project-URL: Github, https://github.com/PrivatePandaCO/pyloggor
```

### Comparing `pyloggor-1.1.2/README.md` & `pyloggor-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyloggor-1.1.2/pyloggor/pyloggor.py` & `pyloggor-1.1.3/pyloggor/pyloggor.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         console_output=True,
         level_colours: dict = default_level_colours,
         default_colour="\033[1;37m",
         delim="|",
         datefmt=r"%d-%b-%y, %H:%M:%S:%f",
         level_symbols=default_level_symbols,
         auto_filename=True,
+        project_root="",
         show_file=True,
         show_symbol=True,
         show_time=True,
         show_topic=True,
         title_level=False,
         file_log_freq=3,
     ):
@@ -84,14 +85,15 @@
         self.level_symbols = level_symbols
 
         self.level_colours = level_colours
         self.default_colour = default_colour
         self.delim = delim
         self.datefmt = datefmt
 
+        self.project_root = project_root
         self.auto_filename = auto_filename
         self.show_file = show_file
         self.show_symbol = show_symbol
         self.show_time = show_time
         self.show_topic = show_topic
         self.title_level = title_level
 
@@ -150,16 +152,29 @@
             _msg += f"[{level_symbol}] "
 
         if self.show_time:
             _msg += f"{time_str} {self.delim} "
         _msg += f"{self.beautify(level, self.level_adjustment_space, self.center_level)} {self.delim} "
         if self.show_file:
             if self.auto_filename:
+                # a very weird way of finding the right rel path given project root
                 frame = inspect.currentframe().f_back
-                file = f"{os.path.relpath(frame.f_code.co_filename, start=os.getcwd())}:{frame.f_lineno}"
+                filename = frame.f_code.co_filename
+                current_dir = os.path.dirname(filename)
+
+                while True:
+                    if os.path.basename(current_dir) == self.project_root:
+                        break
+                    parent_dir = os.path.dirname(current_dir)
+                    if parent_dir == current_dir:  # Reached the filesystem root
+                        break
+                    current_dir = parent_dir
+
+                file = f"{os.path.join(os.path.basename(current_dir), os.path.relpath(filename, start=current_dir))}:{frame.f_lineno}"
+
             _msg += f"{self.beautify(file, self.file_adjustment_space, self.center_file)} {self.delim} "
         if self.show_topic:
             _msg += f"{self.beautify(topic, self.topic_adjustment_space, self.center_topic)} {self.delim} "
         _msg += f"{msg} {extras_str}"
 
         if level.upper() in self.level_colours.keys():
             level_colour = self.level_colours[level.upper()]
```

### Comparing `pyloggor-1.1.2/pyloggor.egg-info/PKG-INFO` & `pyloggor-1.1.3/pyloggor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyloggor
-Version: 1.1.2
+Version: 1.1.3
 Summary: An incredibly versatile yet simple logging system.
 Home-page: https://www.github.com/PrivatePandaCO/pyloggor
 Author: Parth Mittal
 Author-email: parth@privatepanda.co
 License: MIT
 Project-URL: Documentation, https://github.com/PrivatePandaCO/pyloggor/blob/master/README.md
 Project-URL: Github, https://github.com/PrivatePandaCO/pyloggor
```

### Comparing `pyloggor-1.1.2/setup.py` & `pyloggor-1.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name="pyloggor",
-    version="1.1.2",
+    version="1.1.3",
     description="An incredibly versatile yet simple logging system.",
     author="Parth Mittal",
     author_email="parth@privatepanda.co",
     url="https://www.github.com/PrivatePandaCO/pyloggor",
     license="MIT",
     packages=["pyloggor"],
     install_requires=["pytz"],
```

