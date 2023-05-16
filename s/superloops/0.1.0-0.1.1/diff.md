# Comparing `tmp/superloops-0.1.0.tar.gz` & `tmp/superloops-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\superloops-0.1.0.tar", last modified: Tue May 16 19:53:25 2023, max compression
+gzip compressed data, was "dist\superloops-0.1.1.tar", last modified: Tue May 16 23:24:58 2023, max compression
```

## Comparing `superloops-0.1.0.tar` & `superloops-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 19:53:25.000000 superloops-0.1.0/
--rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 superloops-0.1.0/LICENSE
--rw-rw-rw-   0        0        0    11167 2023-05-16 19:53:25.000000 superloops-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    10367 2023-05-16 19:39:55.000000 superloops-0.1.0/README.md
--rw-rw-rw-   0        0        0       86 2023-05-16 19:53:25.000000 superloops-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1287 2023-05-16 19:48:54.000000 superloops-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:53:25.000000 superloops-0.1.0/superloops/
--rw-rw-rw-   0        0        0       23 2023-05-16 19:45:41.000000 superloops-0.1.0/superloops/__init__.py
--rw-rw-rw-   0        0        0    12151 2023-05-16 19:11:39.000000 superloops-0.1.0/superloops/superloops.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:53:25.000000 superloops-0.1.0/superloops.egg-info/
--rw-rw-rw-   0        0        0    11167 2023-05-16 19:53:24.000000 superloops-0.1.0/superloops.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-16 19:53:24.000000 superloops-0.1.0/superloops.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 19:53:24.000000 superloops-0.1.0/superloops.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-16 19:53:24.000000 superloops-0.1.0/superloops.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 19:53:25.000000 superloops-0.1.0/test/
--rw-rw-rw-   0        0        0    16745 2023-05-16 18:53:20.000000 superloops-0.1.0/test/test_superloops.py
+drwxrwxrwx   0        0        0        0 2023-05-16 23:24:58.000000 superloops-0.1.1/
+-rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 superloops-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0    11167 2023-05-16 23:24:58.000000 superloops-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10367 2023-05-16 19:39:55.000000 superloops-0.1.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-16 23:24:58.000000 superloops-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1287 2023-05-16 19:48:54.000000 superloops-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 23:24:58.000000 superloops-0.1.1/superloops/
+-rw-rw-rw-   0        0        0       60 2023-05-16 23:24:41.000000 superloops-0.1.1/superloops/__init__.py
+-rw-rw-rw-   0        0        0    12151 2023-05-16 19:11:39.000000 superloops-0.1.1/superloops/superloops.py
+drwxrwxrwx   0        0        0        0 2023-05-16 23:24:58.000000 superloops-0.1.1/superloops.egg-info/
+-rw-rw-rw-   0        0        0    11167 2023-05-16 23:24:57.000000 superloops-0.1.1/superloops.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-16 23:24:57.000000 superloops-0.1.1/superloops.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 23:24:57.000000 superloops-0.1.1/superloops.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-16 23:24:57.000000 superloops-0.1.1/superloops.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 23:24:58.000000 superloops-0.1.1/test/
+-rw-rw-rw-   0        0        0    16745 2023-05-16 18:53:20.000000 superloops-0.1.1/test/test_superloops.py
```

### Comparing `superloops-0.1.0/LICENSE` & `superloops-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `superloops-0.1.0/PKG-INFO` & `superloops-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superloops
-Version: 0.1.0
+Version: 0.1.1
 Summary: SuperLoops package simplifies and augments usage of Python threads. It provides support for thread maintenance, events, failure handling, health status propagation, and graceful termination.
 Home-page: https://github.com/Voyz/superloops
 Author: Voy Zan
 Author-email: voy1982@yahoo.co.uk
 License: Apache-2.0
 Keywords: thread,threads,python threads,threading,multithreading,asynchronous,concurrency,thread management
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superloops Version: 0.1.0 Summary: SuperLoops
+Metadata-Version: 2.1 Name: superloops Version: 0.1.1 Summary: SuperLoops
 package simplifies and augments usage of Python threads. It provides support
 for thread maintenance, events, failure handling, health status propagation,
 and graceful termination. Home-page: https://github.com/Voyz/superloops Author:
 Voy Zan Author-email: voy1982@yahoo.co.uk License: Apache-2.0 Keywords:
 thread,threads,python
 threads,threading,multithreading,asynchronous,concurrency,thread management
 Platform: UNKNOWN Classifier: Development Status :: 4 - Beta Classifier:
```

### Comparing `superloops-0.1.0/README.md` & `superloops-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `superloops-0.1.0/setup.py` & `superloops-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `superloops-0.1.0/superloops/superloops.py` & `superloops-0.1.1/superloops/superloops.py`

 * *Files identical despite different names*

### Comparing `superloops-0.1.0/superloops.egg-info/PKG-INFO` & `superloops-0.1.1/superloops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superloops
-Version: 0.1.0
+Version: 0.1.1
 Summary: SuperLoops package simplifies and augments usage of Python threads. It provides support for thread maintenance, events, failure handling, health status propagation, and graceful termination.
 Home-page: https://github.com/Voyz/superloops
 Author: Voy Zan
 Author-email: voy1982@yahoo.co.uk
 License: Apache-2.0
 Keywords: thread,threads,python threads,threading,multithreading,asynchronous,concurrency,thread management
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superloops Version: 0.1.0 Summary: SuperLoops
+Metadata-Version: 2.1 Name: superloops Version: 0.1.1 Summary: SuperLoops
 package simplifies and augments usage of Python threads. It provides support
 for thread maintenance, events, failure handling, health status propagation,
 and graceful termination. Home-page: https://github.com/Voyz/superloops Author:
 Voy Zan Author-email: voy1982@yahoo.co.uk License: Apache-2.0 Keywords:
 thread,threads,python
 threads,threading,multithreading,asynchronous,concurrency,thread management
 Platform: UNKNOWN Classifier: Development Status :: 4 - Beta Classifier:
```

### Comparing `superloops-0.1.0/test/test_superloops.py` & `superloops-0.1.1/test/test_superloops.py`

 * *Files identical despite different names*

