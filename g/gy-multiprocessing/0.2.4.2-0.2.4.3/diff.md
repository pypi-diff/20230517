# Comparing `tmp/gy_multiprocessing-0.2.4.2.tar.gz` & `tmp/gy_multiprocessing-0.2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gy_multiprocessing-0.2.4.2.tar", last modified: Wed Apr 12 10:20:43 2023, max compression
+gzip compressed data, was "gy_multiprocessing-0.2.4.3.tar", last modified: Wed May 17 15:26:05 2023, max compression
```

## Comparing `gy_multiprocessing-0.2.4.2.tar` & `gy_multiprocessing-0.2.4.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 10:20:43.543997 gy_multiprocessing-0.2.4.2/
--rw-r--r--   0 guangyuhe   (501) staff       (20)     6438 2023-04-12 10:20:43.543877 gy_multiprocessing-0.2.4.2/PKG-INFO
--rw-r--r--   0 guangyuhe   (501) staff       (20)     6018 2023-04-12 10:20:23.000000 gy_multiprocessing-0.2.4.2/README.md
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 10:20:43.542547 gy_multiprocessing-0.2.4.2/gy_multiprocessing/
--rw-r--r--   0 guangyuhe   (501) staff       (20)      138 2023-02-22 09:46:14.000000 gy_multiprocessing-0.2.4.2/gy_multiprocessing/__init__.py
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 10:20:43.543430 gy_multiprocessing-0.2.4.2/gy_multiprocessing/multiprocessing/
--rw-r--r--   0 guangyuhe   (501) staff       (20)       61 2023-02-22 09:46:14.000000 gy_multiprocessing-0.2.4.2/gy_multiprocessing/multiprocessing/__init__.py
--rw-r--r--   0 guangyuhe   (501) staff       (20)     7090 2023-04-12 09:23:13.000000 gy_multiprocessing-0.2.4.2/gy_multiprocessing/multiprocessing/multi_process.py
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 10:20:43.543688 gy_multiprocessing-0.2.4.2/gy_multiprocessing/multithreading/
--rw-r--r--   0 guangyuhe   (501) staff       (20)       59 2023-02-22 09:46:14.000000 gy_multiprocessing-0.2.4.2/gy_multiprocessing/multithreading/__init__.py
--rw-r--r--   0 guangyuhe   (501) staff       (20)     2289 2023-02-22 11:22:12.000000 gy_multiprocessing-0.2.4.2/gy_multiprocessing/multithreading/multi_thread.py
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 10:20:43.543168 gy_multiprocessing-0.2.4.2/gy_multiprocessing.egg-info/
--rw-r--r--   0 guangyuhe   (501) staff       (20)     6438 2023-04-12 10:20:43.000000 gy_multiprocessing-0.2.4.2/gy_multiprocessing.egg-info/PKG-INFO
--rw-r--r--   0 guangyuhe   (501) staff       (20)      412 2023-04-12 10:20:43.000000 gy_multiprocessing-0.2.4.2/gy_multiprocessing.egg-info/SOURCES.txt
--rw-r--r--   0 guangyuhe   (501) staff       (20)        1 2023-04-12 10:20:43.000000 gy_multiprocessing-0.2.4.2/gy_multiprocessing.egg-info/dependency_links.txt
--rw-r--r--   0 guangyuhe   (501) staff       (20)       19 2023-04-12 10:20:43.000000 gy_multiprocessing-0.2.4.2/gy_multiprocessing.egg-info/top_level.txt
--rw-r--r--   0 guangyuhe   (501) staff       (20)       38 2023-04-12 10:20:43.544032 gy_multiprocessing-0.2.4.2/setup.cfg
--rw-r--r--   0 guangyuhe   (501) staff       (20)      826 2023-04-12 10:20:16.000000 gy_multiprocessing-0.2.4.2/setup.py
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-05-17 15:26:05.047311 gy_multiprocessing-0.2.4.3/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     6428 2023-05-17 15:26:05.047198 gy_multiprocessing-0.2.4.3/PKG-INFO
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     6008 2023-05-17 15:25:02.000000 gy_multiprocessing-0.2.4.3/README.md
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-05-17 15:26:05.046207 gy_multiprocessing-0.2.4.3/gy_multiprocessing/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)      184 2023-05-17 15:16:59.000000 gy_multiprocessing-0.2.4.3/gy_multiprocessing/__init__.py
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-05-17 15:26:05.046850 gy_multiprocessing-0.2.4.3/gy_multiprocessing/multiprocessing/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)        0 2023-05-17 15:16:20.000000 gy_multiprocessing-0.2.4.3/gy_multiprocessing/multiprocessing/__init__.py
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     7217 2023-05-17 15:21:24.000000 gy_multiprocessing-0.2.4.3/gy_multiprocessing/multiprocessing/multi_process.py
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-05-17 15:26:05.047037 gy_multiprocessing-0.2.4.3/gy_multiprocessing/multithreading/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)        0 2023-05-17 15:16:59.000000 gy_multiprocessing-0.2.4.3/gy_multiprocessing/multithreading/__init__.py
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     2289 2023-02-22 11:22:12.000000 gy_multiprocessing-0.2.4.3/gy_multiprocessing/multithreading/multi_thread.py
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-05-17 15:26:05.046646 gy_multiprocessing-0.2.4.3/gy_multiprocessing.egg-info/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     6428 2023-05-17 15:26:05.000000 gy_multiprocessing-0.2.4.3/gy_multiprocessing.egg-info/PKG-INFO
+-rw-r--r--   0 guangyuhe   (501) staff       (20)      412 2023-05-17 15:26:05.000000 gy_multiprocessing-0.2.4.3/gy_multiprocessing.egg-info/SOURCES.txt
+-rw-r--r--   0 guangyuhe   (501) staff       (20)        1 2023-05-17 15:26:05.000000 gy_multiprocessing-0.2.4.3/gy_multiprocessing.egg-info/dependency_links.txt
+-rw-r--r--   0 guangyuhe   (501) staff       (20)       19 2023-05-17 15:26:05.000000 gy_multiprocessing-0.2.4.3/gy_multiprocessing.egg-info/top_level.txt
+-rw-r--r--   0 guangyuhe   (501) staff       (20)       38 2023-05-17 15:26:05.047344 gy_multiprocessing-0.2.4.3/setup.cfg
+-rw-r--r--   0 guangyuhe   (501) staff       (20)      826 2023-05-17 15:21:51.000000 gy_multiprocessing-0.2.4.3/setup.py
```

### Comparing `gy_multiprocessing-0.2.4.2/PKG-INFO` & `gy_multiprocessing-0.2.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gy_multiprocessing
-Version: 0.2.4.2
+Version: 0.2.4.3
 Summary: Run function in multiple processes
 Home-page: https://github.com/guangyu-he/gy-multiprocessing
 Author: Guangyu He
 Author-email: me@heguangyu.net
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -41,16 +41,16 @@
 - please attention to the queue implementation when using multiprocessing, details check the example below
 
 ## Examples
 
 ### Multi Processing
 
 ```python
-import gy_multiprocessing.multiprocessing.multi_process as gymp
 import time
+import gy_multiprocessing as gymp
 
 
 def your_func(a_string: int, queue):
     # NOTE! you MUST add an argument for queue and use put() method to fetch the returning value
 
     print(a_string)
     if a_string % 5 == 0:
@@ -91,15 +91,15 @@
     result = mp.run()
     print(result)
 ```
 
 ### Multi Threads
 
 ```python
-import gy_multiprocessing.multithreading.multi_thread as gymt
+import gy_multiprocessing as gymp
 import time
 
 
 def your_func(a_string):
     # your single task function
 
     print(a_string)
@@ -114,15 +114,15 @@
     start = time.time()
 
     """
     # initializing the multithreading instance
     # the default max_threads are your cpu max cores number - 1
     # max_threads can not larger than your cpu max core number
     """
-    mt = gymt.MultiThread(max_threads=4)
+    mt = gymp.MultiThread(max_threads=4)
 
     # example for multithreading in the loop
     outer_loop_times = 5
     for current_loop_index in range(outer_loop_times):
         args = (str(current_loop_index),)
 
         """
@@ -151,31 +151,30 @@
 
 <b>Note: you can not use multiprocessing or sub-multithreading in the multithreading method</b>
 
 If you want to use such structure, based on your needs, considering using sub-multiprocessing or multithreading in
 multiprocessing structure.
 
 ```python
-import gy_multiprocessing.multiprocessing.multi_process as gymp
-import gy_multiprocessing.multithreading.multi_thread as gymt
+import gy_multiprocessing as gymp
 
 
 def your_sub_func(b_string: int, queue=None):
     # your function that needs to multithreading/multiprocessing
 
     b_string += 1
     if queue is not None:
         queue.put(b_string)
     return b_string
 
 
 def your_mt_func(a_string: int, queue):
     # multithreading in multiprocessing structure
 
-    mt = gymt.MultiThread()
+    mt = gymp.MultiThread()
     for current_loop_index in range(a_string):
         # your running arguments, must be tuple
         args = (current_loop_index,)
         mt.add(your_sub_func, args)
     result = mt.run()
 
     # Do not forget queue!
@@ -238,14 +237,21 @@
 
 - fixed an issue from readme long desc causing installation error
 
 #### improvement
 
 - simplified duplicated codes
 
+### v0.2.4.3
+
+#### updates
+
+- package import improvement. **PLEASE UPDATE IMPORT AS EXAMPLES ABOVE**
+- check a boolean type input argument
+
 ## Support
 
 feel free to check source code in <a href="https://github.com/guangyu-he/gy-multiprocessing">GitHub</a>, you are welcome
 to leave any comments.
 
 2022&copy;Guangyu He, for further support please contact author. <br>
 Email: <a href="mailto:me@heguangyu.net">me@heguangyu.net</a>
```

### Comparing `gy_multiprocessing-0.2.4.2/README.md` & `gy_multiprocessing-0.2.4.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 - please attention to the queue implementation when using multiprocessing, details check the example below
 
 ## Examples
 
 ### Multi Processing
 
 ```python
-import gy_multiprocessing.multiprocessing.multi_process as gymp
 import time
+import gy_multiprocessing as gymp
 
 
 def your_func(a_string: int, queue):
     # NOTE! you MUST add an argument for queue and use put() method to fetch the returning value
 
     print(a_string)
     if a_string % 5 == 0:
@@ -78,15 +78,15 @@
     result = mp.run()
     print(result)
 ```
 
 ### Multi Threads
 
 ```python
-import gy_multiprocessing.multithreading.multi_thread as gymt
+import gy_multiprocessing as gymp
 import time
 
 
 def your_func(a_string):
     # your single task function
 
     print(a_string)
@@ -101,15 +101,15 @@
     start = time.time()
 
     """
     # initializing the multithreading instance
     # the default max_threads are your cpu max cores number - 1
     # max_threads can not larger than your cpu max core number
     """
-    mt = gymt.MultiThread(max_threads=4)
+    mt = gymp.MultiThread(max_threads=4)
 
     # example for multithreading in the loop
     outer_loop_times = 5
     for current_loop_index in range(outer_loop_times):
         args = (str(current_loop_index),)
 
         """
@@ -138,31 +138,30 @@
 
 <b>Note: you can not use multiprocessing or sub-multithreading in the multithreading method</b>
 
 If you want to use such structure, based on your needs, considering using sub-multiprocessing or multithreading in
 multiprocessing structure.
 
 ```python
-import gy_multiprocessing.multiprocessing.multi_process as gymp
-import gy_multiprocessing.multithreading.multi_thread as gymt
+import gy_multiprocessing as gymp
 
 
 def your_sub_func(b_string: int, queue=None):
     # your function that needs to multithreading/multiprocessing
 
     b_string += 1
     if queue is not None:
         queue.put(b_string)
     return b_string
 
 
 def your_mt_func(a_string: int, queue):
     # multithreading in multiprocessing structure
 
-    mt = gymt.MultiThread()
+    mt = gymp.MultiThread()
     for current_loop_index in range(a_string):
         # your running arguments, must be tuple
         args = (current_loop_index,)
         mt.add(your_sub_func, args)
     result = mt.run()
 
     # Do not forget queue!
@@ -225,14 +224,21 @@
 
 - fixed an issue from readme long desc causing installation error
 
 #### improvement
 
 - simplified duplicated codes
 
+### v0.2.4.3
+
+#### updates
+
+- package import improvement. **PLEASE UPDATE IMPORT AS EXAMPLES ABOVE**
+- check a boolean type input argument
+
 ## Support
 
 feel free to check source code in <a href="https://github.com/guangyu-he/gy-multiprocessing">GitHub</a>, you are welcome
 to leave any comments.
 
 2022&copy;Guangyu He, for further support please contact author. <br>
 Email: <a href="mailto:me@heguangyu.net">me@heguangyu.net</a>
```

### Comparing `gy_multiprocessing-0.2.4.2/gy_multiprocessing/multiprocessing/multi_process.py` & `gy_multiprocessing-0.2.4.3/gy_multiprocessing/multiprocessing/multi_process.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,19 @@
         Using Process method from multiprocessing to process the multiprocessing tasks
         """
 
         # error handling
         if type(max_process) is not int:
             raise TypeError(f"Wrong type of max process '{max_process}', must be an integer!")
         if max_process == 0:
-            raise IndexError("max process are set to be 0!")
+            raise IndexError("max process can not be 0!")
         if max_process > cpu_count():
             warnings.warn("too much sub processes, performance may get influenced!")
+        if isinstance(silent, bool) is False:
+            raise TypeError(f"Wrong type of silent '{silent}', must be a boolean!")
 
         # set max processing pool equals to the cpu core number
         self.max_process: int = max_process
 
         # show log in console
         self.silent: bool = silent
```

### Comparing `gy_multiprocessing-0.2.4.2/gy_multiprocessing/multithreading/multi_thread.py` & `gy_multiprocessing-0.2.4.3/gy_multiprocessing/multithreading/multi_thread.py`

 * *Files identical despite different names*

### Comparing `gy_multiprocessing-0.2.4.2/gy_multiprocessing.egg-info/PKG-INFO` & `gy_multiprocessing-0.2.4.3/gy_multiprocessing.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gy-multiprocessing
-Version: 0.2.4.2
+Version: 0.2.4.3
 Summary: Run function in multiple processes
 Home-page: https://github.com/guangyu-he/gy-multiprocessing
 Author: Guangyu He
 Author-email: me@heguangyu.net
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -41,16 +41,16 @@
 - please attention to the queue implementation when using multiprocessing, details check the example below
 
 ## Examples
 
 ### Multi Processing
 
 ```python
-import gy_multiprocessing.multiprocessing.multi_process as gymp
 import time
+import gy_multiprocessing as gymp
 
 
 def your_func(a_string: int, queue):
     # NOTE! you MUST add an argument for queue and use put() method to fetch the returning value
 
     print(a_string)
     if a_string % 5 == 0:
@@ -91,15 +91,15 @@
     result = mp.run()
     print(result)
 ```
 
 ### Multi Threads
 
 ```python
-import gy_multiprocessing.multithreading.multi_thread as gymt
+import gy_multiprocessing as gymp
 import time
 
 
 def your_func(a_string):
     # your single task function
 
     print(a_string)
@@ -114,15 +114,15 @@
     start = time.time()
 
     """
     # initializing the multithreading instance
     # the default max_threads are your cpu max cores number - 1
     # max_threads can not larger than your cpu max core number
     """
-    mt = gymt.MultiThread(max_threads=4)
+    mt = gymp.MultiThread(max_threads=4)
 
     # example for multithreading in the loop
     outer_loop_times = 5
     for current_loop_index in range(outer_loop_times):
         args = (str(current_loop_index),)
 
         """
@@ -151,31 +151,30 @@
 
 <b>Note: you can not use multiprocessing or sub-multithreading in the multithreading method</b>
 
 If you want to use such structure, based on your needs, considering using sub-multiprocessing or multithreading in
 multiprocessing structure.
 
 ```python
-import gy_multiprocessing.multiprocessing.multi_process as gymp
-import gy_multiprocessing.multithreading.multi_thread as gymt
+import gy_multiprocessing as gymp
 
 
 def your_sub_func(b_string: int, queue=None):
     # your function that needs to multithreading/multiprocessing
 
     b_string += 1
     if queue is not None:
         queue.put(b_string)
     return b_string
 
 
 def your_mt_func(a_string: int, queue):
     # multithreading in multiprocessing structure
 
-    mt = gymt.MultiThread()
+    mt = gymp.MultiThread()
     for current_loop_index in range(a_string):
         # your running arguments, must be tuple
         args = (current_loop_index,)
         mt.add(your_sub_func, args)
     result = mt.run()
 
     # Do not forget queue!
@@ -238,14 +237,21 @@
 
 - fixed an issue from readme long desc causing installation error
 
 #### improvement
 
 - simplified duplicated codes
 
+### v0.2.4.3
+
+#### updates
+
+- package import improvement. **PLEASE UPDATE IMPORT AS EXAMPLES ABOVE**
+- check a boolean type input argument
+
 ## Support
 
 feel free to check source code in <a href="https://github.com/guangyu-he/gy-multiprocessing">GitHub</a>, you are welcome
 to leave any comments.
 
 2022&copy;Guangyu He, for further support please contact author. <br>
 Email: <a href="mailto:me@heguangyu.net">me@heguangyu.net</a>
```

### Comparing `gy_multiprocessing-0.2.4.2/setup.py` & `gy_multiprocessing-0.2.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = Path(__file__).parent
 with open(this_directory / "README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="gy_multiprocessing",
-    version="0.2.4.2",
+    version="0.2.4.3",
     author="Guangyu He",
     author_email="me@heguangyu.net",
     description="Run function in multiple processes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/guangyu-he/gy-multiprocessing",
     install_requires=[],
```

