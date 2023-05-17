# Comparing `tmp/jiujitsu-0.5.tar.gz` & `tmp/jiujitsu-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiujitsu-0.5.tar", last modified: Wed May 17 16:09:11 2023, max compression
+gzip compressed data, was "jiujitsu-0.6.tar", last modified: Wed May 17 16:37:50 2023, max compression
```

## Comparing `jiujitsu-0.5.tar` & `jiujitsu-0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:09:11.757191 jiujitsu-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-17 16:09:11.757191 jiujitsu-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-05-17 16:08:58.000000 jiujitsu-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:09:11.753191 jiujitsu-0.5/jiujitsu/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/bpFileSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/bpInterpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)    31394 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/bpInterpreterBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/bpPrimitives.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24426 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/jInterpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/jNode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/jParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/jRecord.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:09:11.753191 jiujitsu-0.5/jiujitsu/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/test/test_bpInterpreterBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/test/test_bpPrimitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/test/test_jInterpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/test/test_jParser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:09:11.753191 jiujitsu-0.5/jiujitsu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-17 16:09:11.000000 jiujitsu-0.5/jiujitsu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-17 16:09:11.000000 jiujitsu-0.5/jiujitsu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:09:11.000000 jiujitsu-0.5/jiujitsu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-17 16:09:11.000000 jiujitsu-0.5/jiujitsu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 16:09:11.000000 jiujitsu-0.5/jiujitsu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 16:09:11.000000 jiujitsu-0.5/jiujitsu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-17 16:09:11.757191 jiujitsu-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-17 16:08:58.000000 jiujitsu-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:37:50.625013 jiujitsu-0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-17 16:37:50.625013 jiujitsu-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-05-17 16:37:34.000000 jiujitsu-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:37:50.625013 jiujitsu-0.6/jiujitsu/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-17 16:37:34.000000 jiujitsu-0.6/jiujitsu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-17 16:37:34.000000 jiujitsu-0.6/jiujitsu/bpFileSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-17 16:37:34.000000 jiujitsu-0.6/jiujitsu/bpInterpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31394 2023-05-17 16:37:34.000000 jiujitsu-0.6/jiujitsu/bpInterpreterBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-05-17 16:37:34.000000 jiujitsu-0.6/jiujitsu/bpPrimitives.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24426 2023-05-17 16:37:34.000000 jiujitsu-0.6/jiujitsu/jInterpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-17 16:37:34.000000 jiujitsu-0.6/jiujitsu/jNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-17 16:37:34.000000 jiujitsu-0.6/jiujitsu/jParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-17 16:37:34.000000 jiujitsu-0.6/jiujitsu/jRecord.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:37:50.625013 jiujitsu-0.6/jiujitsu/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:37:34.000000 jiujitsu-0.6/jiujitsu/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-05-17 16:37:34.000000 jiujitsu-0.6/jiujitsu/test/test_bpInterpreterBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-05-17 16:37:34.000000 jiujitsu-0.6/jiujitsu/test/test_bpPrimitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-05-17 16:37:34.000000 jiujitsu-0.6/jiujitsu/test/test_jInterpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-17 16:37:34.000000 jiujitsu-0.6/jiujitsu/test/test_jParser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:37:50.625013 jiujitsu-0.6/jiujitsu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-17 16:37:50.000000 jiujitsu-0.6/jiujitsu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-17 16:37:50.000000 jiujitsu-0.6/jiujitsu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:37:50.000000 jiujitsu-0.6/jiujitsu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-17 16:37:50.000000 jiujitsu-0.6/jiujitsu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 16:37:50.000000 jiujitsu-0.6/jiujitsu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 16:37:50.000000 jiujitsu-0.6/jiujitsu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-17 16:37:50.625013 jiujitsu-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-17 16:37:34.000000 jiujitsu-0.6/setup.py
```

### Comparing `jiujitsu-0.5/README.md` & `jiujitsu-0.6/README.md`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.5/jiujitsu/__init__.py` & `jiujitsu-0.6/jiujitsu/__init__.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.5/jiujitsu/bpFileSystem.py` & `jiujitsu-0.6/jiujitsu/bpFileSystem.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.5/jiujitsu/bpInterpreter.py` & `jiujitsu-0.6/jiujitsu/bpInterpreter.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.5/jiujitsu/bpInterpreterBase.py` & `jiujitsu-0.6/jiujitsu/bpInterpreterBase.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.5/jiujitsu/bpPrimitives.py` & `jiujitsu-0.6/jiujitsu/bpPrimitives.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,15 @@
 
     def functionsText(self):
         output = 'Functions: \n'
         for name, node in self.functions.items():
             output += '  ' + name + ':\n'
             node_text = '     ' + str(bashparser.NodeVisitor(node))
             node_text = node_text.replace('\n', '\n    ')  # auto indent properly
-            output += node_text
+            output += node_text + '\n'
             #for node in nodes:
             #    output += '    ' + str(NodeVisitor(node)) + '\n'
         if not len(self.functions):
             output += '  No functions in list\n'
         return output
 
     def showFunctions(self):
```

### Comparing `jiujitsu-0.5/jiujitsu/jInterpreter.py` & `jiujitsu-0.6/jiujitsu/jInterpreter.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.5/jiujitsu/jNode.py` & `jiujitsu-0.6/jiujitsu/jNode.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.5/jiujitsu/jParser.py` & `jiujitsu-0.6/jiujitsu/jParser.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.5/jiujitsu/jRecord.py` & `jiujitsu-0.6/jiujitsu/jRecord.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.5/jiujitsu/test/test_bpInterpreterBase.py` & `jiujitsu-0.6/jiujitsu/test/test_bpInterpreterBase.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.5/jiujitsu/test/test_bpPrimitives.py` & `jiujitsu-0.6/jiujitsu/test/test_bpPrimitives.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.5/jiujitsu/test/test_jInterpreter.py` & `jiujitsu-0.6/jiujitsu/test/test_jInterpreter.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.5/jiujitsu/test/test_jParser.py` & `jiujitsu-0.6/jiujitsu/test/test_jParser.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.5/jiujitsu.egg-info/SOURCES.txt` & `jiujitsu-0.6/jiujitsu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.5/setup.cfg` & `jiujitsu-0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jiujitsu
-version = 0.5
+version = 0.6
 author = Spencer Stingley
 description = A custom bash interpreter for malware execution
 long_description = A custom bash interpreter for malware execution
 url = https://github.com/BlankCanvasStudio/jiujitsu
 keywords = bash, parsing, interpreter, analysis, malware
 python_requires = >=3.6
 classifiers =
```

### Comparing `jiujitsu-0.5/setup.py` & `jiujitsu-0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jiujitsu",
-    version="0.5",
+    version="0.6",
     author="Spencer Stingley",
     author_email="sstingle@usc.edu",
     description="A custom bash interpreter for malware execution",
     long_description="A custom bash interpreter for malware execution",
     long_description_content_type="text/markdown",
     url="https://github.com/BlankCanvasStudio/jiujitsu",
     packages=setuptools.find_packages(),
```

