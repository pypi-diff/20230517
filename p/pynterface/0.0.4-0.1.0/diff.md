# Comparing `tmp/pynterface-0.0.4.tar.gz` & `tmp/pynterface-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynterface-0.0.4.tar", last modified: Wed May 17 03:19:17 2023, max compression
+gzip compressed data, was "pynterface-0.1.0.tar", last modified: Wed May 17 14:26:00 2023, max compression
```

## Comparing `pynterface-0.0.4.tar` & `pynterface-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-17 03:19:17.858839 pynterface-0.0.4/
--rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-05-04 02:59:32.000000 pynterface-0.0.4/LICENSE
--rw-r--r--   0 vivaan     (501) staff       (20)       33 2023-05-14 03:48:17.000000 pynterface-0.0.4/MANIFEST.in
--rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-05-17 03:19:17.858522 pynterface-0.0.4/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)     1156 2023-05-14 04:10:04.000000 pynterface-0.0.4/README.md
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-17 03:19:17.856767 pynterface-0.0.4/pynterface/
--rw-r--r--   0 vivaan     (501) staff       (20)      238 2023-05-17 03:18:45.000000 pynterface-0.0.4/pynterface/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     2840 2023-05-15 19:24:45.000000 pynterface-0.0.4/pynterface/input.py
--rw-r--r--   0 vivaan     (501) staff       (20)     6541 2023-05-17 03:18:29.000000 pynterface-0.0.4/pynterface/loading.py
--rw-r--r--   0 vivaan     (501) staff       (20)     3367 2023-05-15 15:05:04.000000 pynterface-0.0.4/pynterface/menu.py
--rw-r--r--   0 vivaan     (501) staff       (20)     5444 2023-05-14 18:25:39.000000 pynterface-0.0.4/pynterface/printing.py
--rw-r--r--   0 vivaan     (501) staff       (20)     5848 2023-05-15 14:51:42.000000 pynterface-0.0.4/pynterface/style.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-17 03:19:17.858119 pynterface-0.0.4/pynterface.egg-info/
--rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-05-17 03:19:17.000000 pynterface-0.0.4/pynterface.egg-info/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)      301 2023-05-17 03:19:17.000000 pynterface-0.0.4/pynterface.egg-info/SOURCES.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-17 03:19:17.000000 pynterface-0.0.4/pynterface.egg-info/dependency_links.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       11 2023-05-17 03:19:17.000000 pynterface-0.0.4/pynterface.egg-info/top_level.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-17 03:19:17.858932 pynterface-0.0.4/setup.cfg
--rw-r--r--   0 vivaan     (501) staff       (20)      612 2023-05-14 04:04:56.000000 pynterface-0.0.4/setup.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-17 14:26:00.398145 pynterface-0.1.0/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-05-04 02:59:32.000000 pynterface-0.1.0/LICENSE
+-rw-r--r--   0 vivaan     (501) staff       (20)       33 2023-05-14 03:48:17.000000 pynterface-0.1.0/MANIFEST.in
+-rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-05-17 14:26:00.397839 pynterface-0.1.0/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)     1156 2023-05-14 04:10:04.000000 pynterface-0.1.0/README.md
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-17 14:26:00.396261 pynterface-0.1.0/pynterface/
+-rw-r--r--   0 vivaan     (501) staff       (20)      238 2023-05-17 14:23:19.000000 pynterface-0.1.0/pynterface/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     2840 2023-05-15 19:24:45.000000 pynterface-0.1.0/pynterface/input.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     6438 2023-05-17 14:21:57.000000 pynterface-0.1.0/pynterface/loading.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     3367 2023-05-15 15:05:04.000000 pynterface-0.1.0/pynterface/menu.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     5444 2023-05-14 18:25:39.000000 pynterface-0.1.0/pynterface/printing.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     5848 2023-05-15 14:51:42.000000 pynterface-0.1.0/pynterface/style.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-17 14:26:00.397408 pynterface-0.1.0/pynterface.egg-info/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-05-17 14:26:00.000000 pynterface-0.1.0/pynterface.egg-info/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)      301 2023-05-17 14:26:00.000000 pynterface-0.1.0/pynterface.egg-info/SOURCES.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-17 14:26:00.000000 pynterface-0.1.0/pynterface.egg-info/dependency_links.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       11 2023-05-17 14:26:00.000000 pynterface-0.1.0/pynterface.egg-info/top_level.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-17 14:26:00.398230 pynterface-0.1.0/setup.cfg
+-rw-r--r--   0 vivaan     (501) staff       (20)      612 2023-05-14 04:04:56.000000 pynterface-0.1.0/setup.py
```

### Comparing `pynterface-0.0.4/LICENSE` & `pynterface-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.4/PKG-INFO` & `pynterface-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynterface
-Version: 0.0.4
+Version: 0.1.0
 Summary: Terminal-Based Printing Tools!
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://pynterface.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pynterface-0.0.4/README.md` & `pynterface-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.4/pynterface/input.py` & `pynterface-0.1.0/pynterface/input.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.4/pynterface/loading.py` & `pynterface-0.1.0/pynterface/loading.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,25 +27,22 @@
 
         assert all([isinstance(part, str) for part in cycle]), "Cycle must consist of strings only."
         assert isinstance(message, str), "Message must be a string."
 
         self.max_len = max([len(item) for item in cycle])
 
         # stores customization values
-        self.cycle = cycle
+        self.cycle = [item + " " * (self.max_len - len(item)) for item in cycle]
         self.message = message
         self.delay = delay / 1000
         self.hide_cursor = hide_cursor
 
         # temporary null value 
         self.runner = None
 
-        # stores values for going back and clearing
-        self.prev_length = len(self.cycle[0]) 
-        
         # for cycling
         self.mod = len(cycle)
         self.index = 0
 
         # for states
         self.over = False
         self.paused = False
@@ -77,15 +74,14 @@
             print("\033[?25h", end="")  # shows cursor no matter what
 
     def __display(self, item):
         """
         Clears and displays the message.
         """
         self.__clear_animated()
-        self.prev_length = len(item)
         print("\r" + self.message + item, end="")
         stdout.flush()
 
     def __enter__(self) -> Loader:
         self.runner = Thread(target=self.__run)
         self.runner.start()
         return self
@@ -119,17 +115,17 @@
         self.__display(self.cycle[self.__state])
         sleep(self.delay)
 
     def __clear_animated(self):
         """
         Clears the animated thing.
         """
-        print("\b" * self.prev_length 
-              + " " * self.prev_length 
-              + "\b" * self.prev_length, end="")
+        print("\b" * self.max_len 
+              + " " * self.max_len 
+              + "\b" * self.max_len, end="")
 
     def __clear(self):
         """
         Clears the message.
         """
         print("\r" + " " * (len(self.message) + self.max_len + 1), end="")
```

### Comparing `pynterface-0.0.4/pynterface/menu.py` & `pynterface-0.1.0/pynterface/menu.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.4/pynterface/printing.py` & `pynterface-0.1.0/pynterface/printing.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.4/pynterface/style.py` & `pynterface-0.1.0/pynterface/style.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.4/pynterface.egg-info/PKG-INFO` & `pynterface-0.1.0/pynterface.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynterface
-Version: 0.0.4
+Version: 0.1.0
 Summary: Terminal-Based Printing Tools!
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://pynterface.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pynterface-0.0.4/setup.py` & `pynterface-0.1.0/setup.py`

 * *Files identical despite different names*

