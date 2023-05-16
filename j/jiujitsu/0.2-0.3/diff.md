# Comparing `tmp/jiujitsu-0.2.tar.gz` & `tmp/jiujitsu-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiujitsu-0.2.tar", last modified: Tue May 16 21:39:08 2023, max compression
+gzip compressed data, was "jiujitsu-0.3.tar", last modified: Tue May 16 22:36:13 2023, max compression
```

## Comparing `jiujitsu-0.2.tar` & `jiujitsu-0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 adam      (1000) users      (984)        0 2023-05-16 21:39:08.446642 jiujitsu-0.2/
--rw-r--r--   0 adam      (1000) users      (984)      479 2023-05-16 21:39:08.446642 jiujitsu-0.2/PKG-INFO
--rw-r--r--   0 adam      (1000) users      (984)     6367 2023-05-16 16:51:46.000000 jiujitsu-0.2/README.md
-drwxr-xr-x   0 adam      (1000) users      (984)        0 2023-05-16 21:39:08.446642 jiujitsu-0.2/jiujitsu/
--rw-r--r--   0 adam      (1000) users      (984)      515 2023-05-16 17:27:01.000000 jiujitsu-0.2/jiujitsu/__init__.py
--rw-r--r--   0 adam      (1000) users      (984)     1669 2023-05-16 16:52:45.000000 jiujitsu-0.2/jiujitsu/bpFileSystem.py
--rw-r--r--   0 adam      (1000) users      (984)     4535 2023-05-16 17:17:28.000000 jiujitsu-0.2/jiujitsu/bpInterpreter.py
--rw-r--r--   0 adam      (1000) users      (984)    31109 2023-05-16 17:28:34.000000 jiujitsu-0.2/jiujitsu/bpInterpreterBase.py
--rw-r--r--   0 adam      (1000) users      (984)    11559 2023-05-16 17:17:50.000000 jiujitsu-0.2/jiujitsu/bpPrimitives.py
--rwxr-xr-x   0 adam      (1000) users      (984)    24302 2023-05-16 20:09:57.000000 jiujitsu-0.2/jiujitsu/jInterpreter.py
--rw-r--r--   0 adam      (1000) users      (984)     2647 2023-05-16 16:52:45.000000 jiujitsu-0.2/jiujitsu/jNode.py
--rw-r--r--   0 adam      (1000) users      (984)     5163 2023-05-16 17:18:46.000000 jiujitsu-0.2/jiujitsu/jParser.py
--rw-r--r--   0 adam      (1000) users      (984)     1161 2023-05-16 17:18:52.000000 jiujitsu-0.2/jiujitsu/jRecord.py
-drwxr-xr-x   0 adam      (1000) users      (984)        0 2023-05-16 21:39:08.446642 jiujitsu-0.2/jiujitsu/test/
--rw-r--r--   0 adam      (1000) users      (984)        0 2023-05-16 16:51:46.000000 jiujitsu-0.2/jiujitsu/test/__init__.py
--rw-r--r--   0 adam      (1000) users      (984)    14839 2023-05-16 17:21:29.000000 jiujitsu-0.2/jiujitsu/test/test_bpInterpreterBase.py
--rw-r--r--   0 adam      (1000) users      (984)     6025 2023-05-16 17:22:31.000000 jiujitsu-0.2/jiujitsu/test/test_bpPrimitives.py
--rw-r--r--   0 adam      (1000) users      (984)    17534 2023-05-16 17:32:42.000000 jiujitsu-0.2/jiujitsu/test/test_jInterpreter.py
--rw-r--r--   0 adam      (1000) users      (984)      886 2023-05-16 17:25:00.000000 jiujitsu-0.2/jiujitsu/test/test_jParser.py
-drwxr-xr-x   0 adam      (1000) users      (984)        0 2023-05-16 21:39:08.446642 jiujitsu-0.2/jiujitsu.egg-info/
--rw-r--r--   0 adam      (1000) users      (984)      479 2023-05-16 21:39:08.000000 jiujitsu-0.2/jiujitsu.egg-info/PKG-INFO
--rw-r--r--   0 adam      (1000) users      (984)      567 2023-05-16 21:39:08.000000 jiujitsu-0.2/jiujitsu.egg-info/SOURCES.txt
--rw-r--r--   0 adam      (1000) users      (984)        1 2023-05-16 21:39:08.000000 jiujitsu-0.2/jiujitsu.egg-info/dependency_links.txt
--rw-r--r--   0 adam      (1000) users      (984)       50 2023-05-16 21:39:08.000000 jiujitsu-0.2/jiujitsu.egg-info/entry_points.txt
--rw-r--r--   0 adam      (1000) users      (984)        9 2023-05-16 21:39:08.000000 jiujitsu-0.2/jiujitsu.egg-info/top_level.txt
--rw-r--r--   0 adam      (1000) users      (984)      547 2023-05-16 21:39:08.446642 jiujitsu-0.2/setup.cfg
--rw-r--r--   0 adam      (1000) users      (984)      849 2023-05-16 21:38:24.000000 jiujitsu-0.2/setup.py
+drwxr-xr-x   0 adam      (1000) users      (984)        0 2023-05-16 22:36:13.816442 jiujitsu-0.3/
+-rw-r--r--   0 adam      (1000) users      (984)      479 2023-05-16 22:36:13.816442 jiujitsu-0.3/PKG-INFO
+-rw-r--r--   0 adam      (1000) users      (984)     6367 2023-05-16 16:51:46.000000 jiujitsu-0.3/README.md
+drwxr-xr-x   0 adam      (1000) users      (984)        0 2023-05-16 22:36:13.813108 jiujitsu-0.3/jiujitsu/
+-rw-r--r--   0 adam      (1000) users      (984)      515 2023-05-16 17:27:01.000000 jiujitsu-0.3/jiujitsu/__init__.py
+-rw-r--r--   0 adam      (1000) users      (984)     1669 2023-05-16 16:52:45.000000 jiujitsu-0.3/jiujitsu/bpFileSystem.py
+-rw-r--r--   0 adam      (1000) users      (984)     4535 2023-05-16 17:17:28.000000 jiujitsu-0.3/jiujitsu/bpInterpreter.py
+-rw-r--r--   0 adam      (1000) users      (984)    31109 2023-05-16 17:28:34.000000 jiujitsu-0.3/jiujitsu/bpInterpreterBase.py
+-rw-r--r--   0 adam      (1000) users      (984)    11559 2023-05-16 17:17:50.000000 jiujitsu-0.3/jiujitsu/bpPrimitives.py
+-rwxr-xr-x   0 adam      (1000) users      (984)    24302 2023-05-16 20:09:57.000000 jiujitsu-0.3/jiujitsu/jInterpreter.py
+-rw-r--r--   0 adam      (1000) users      (984)     2647 2023-05-16 16:52:45.000000 jiujitsu-0.3/jiujitsu/jNode.py
+-rw-r--r--   0 adam      (1000) users      (984)     5163 2023-05-16 17:18:46.000000 jiujitsu-0.3/jiujitsu/jParser.py
+-rw-r--r--   0 adam      (1000) users      (984)     1161 2023-05-16 17:18:52.000000 jiujitsu-0.3/jiujitsu/jRecord.py
+drwxr-xr-x   0 adam      (1000) users      (984)        0 2023-05-16 22:36:13.816442 jiujitsu-0.3/jiujitsu/test/
+-rw-r--r--   0 adam      (1000) users      (984)        0 2023-05-16 16:51:46.000000 jiujitsu-0.3/jiujitsu/test/__init__.py
+-rw-r--r--   0 adam      (1000) users      (984)    14839 2023-05-16 17:21:29.000000 jiujitsu-0.3/jiujitsu/test/test_bpInterpreterBase.py
+-rw-r--r--   0 adam      (1000) users      (984)     6025 2023-05-16 17:22:31.000000 jiujitsu-0.3/jiujitsu/test/test_bpPrimitives.py
+-rw-r--r--   0 adam      (1000) users      (984)    17534 2023-05-16 17:32:42.000000 jiujitsu-0.3/jiujitsu/test/test_jInterpreter.py
+-rw-r--r--   0 adam      (1000) users      (984)      886 2023-05-16 17:25:00.000000 jiujitsu-0.3/jiujitsu/test/test_jParser.py
+drwxr-xr-x   0 adam      (1000) users      (984)        0 2023-05-16 22:36:13.813108 jiujitsu-0.3/jiujitsu.egg-info/
+-rw-r--r--   0 adam      (1000) users      (984)      479 2023-05-16 22:36:13.000000 jiujitsu-0.3/jiujitsu.egg-info/PKG-INFO
+-rw-r--r--   0 adam      (1000) users      (984)      567 2023-05-16 22:36:13.000000 jiujitsu-0.3/jiujitsu.egg-info/SOURCES.txt
+-rw-r--r--   0 adam      (1000) users      (984)        1 2023-05-16 22:36:13.000000 jiujitsu-0.3/jiujitsu.egg-info/dependency_links.txt
+-rw-r--r--   0 adam      (1000) users      (984)       50 2023-05-16 22:36:13.000000 jiujitsu-0.3/jiujitsu.egg-info/entry_points.txt
+-rw-r--r--   0 adam      (1000) users      (984)        9 2023-05-16 22:36:13.000000 jiujitsu-0.3/jiujitsu.egg-info/top_level.txt
+-rw-r--r--   0 adam      (1000) users      (984)      590 2023-05-16 22:36:13.816442 jiujitsu-0.3/setup.cfg
+-rw-r--r--   0 adam      (1000) users      (984)      897 2023-05-16 22:35:51.000000 jiujitsu-0.3/setup.py
```

### Comparing `jiujitsu-0.2/README.md` & `jiujitsu-0.3/README.md`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.2/jiujitsu/__init__.py` & `jiujitsu-0.3/jiujitsu/__init__.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.2/jiujitsu/bpFileSystem.py` & `jiujitsu-0.3/jiujitsu/bpFileSystem.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.2/jiujitsu/bpInterpreter.py` & `jiujitsu-0.3/jiujitsu/bpInterpreter.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.2/jiujitsu/bpInterpreterBase.py` & `jiujitsu-0.3/jiujitsu/bpInterpreterBase.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.2/jiujitsu/bpPrimitives.py` & `jiujitsu-0.3/jiujitsu/bpPrimitives.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.2/jiujitsu/jInterpreter.py` & `jiujitsu-0.3/jiujitsu/jInterpreter.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.2/jiujitsu/jNode.py` & `jiujitsu-0.3/jiujitsu/jNode.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.2/jiujitsu/jParser.py` & `jiujitsu-0.3/jiujitsu/jParser.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.2/jiujitsu/jRecord.py` & `jiujitsu-0.3/jiujitsu/jRecord.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.2/jiujitsu/test/test_bpInterpreterBase.py` & `jiujitsu-0.3/jiujitsu/test/test_bpInterpreterBase.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.2/jiujitsu/test/test_bpPrimitives.py` & `jiujitsu-0.3/jiujitsu/test/test_bpPrimitives.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.2/jiujitsu/test/test_jInterpreter.py` & `jiujitsu-0.3/jiujitsu/test/test_jInterpreter.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.2/jiujitsu/test/test_jParser.py` & `jiujitsu-0.3/jiujitsu/test/test_jParser.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.2/jiujitsu.egg-info/SOURCES.txt` & `jiujitsu-0.3/jiujitsu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.2/setup.cfg` & `jiujitsu-0.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [metadata]
 name = jiujitsu
-version = 0.2
+version = 0.3
 author = Spencer Stingley
 description = A custom bash interpreter for malware execution
 long_description = A custom bash interpreter for malware execution
 url = https://github.com/BlankCanvasStudio/jiujitsu
 keywords = bash, parsing, interpreter, analysis, malware
 python_requires = >=3.6
 classifiers = 
 	Programming Language :: Python :: 3
 	Operating System :: OS Independent
+install_requires = [ bashlex, bashparser ]
 test = 
 	nose2
 
 [options.entry_points]
 console_scripts = 
 	jj = jiujitsu.jInterpreter:main
```

### Comparing `jiujitsu-0.2/setup.py` & `jiujitsu-0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jiujitsu",
-    version="0.2",
+    version="0.3",
     author="Spencer Stingley",
     author_email="sstingle@usc.edu",
     description="A custom bash interpreter for malware execution",
     long_description="A custom bash interpreter for malware execution",
     long_description_content_type="text/markdown",
     url="https://github.com/BlankCanvasStudio/jiujitsu",
     packages=setuptools.find_packages(),
@@ -21,10 +21,11 @@
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     python_requires = '>=3.6',
+    requires_install=['bashlex', 'bashparser'],
     test_suite='nose.collector',
     tests_require=['nose'],
 )
```

