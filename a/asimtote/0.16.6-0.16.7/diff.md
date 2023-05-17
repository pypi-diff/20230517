# Comparing `tmp/asimtote-0.16.6.tar.gz` & `tmp/asimtote-0.16.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asimtote-0.16.6.tar", last modified: Mon Apr 17 14:16:03 2023, max compression
+gzip compressed data, was "asimtote-0.16.7.tar", last modified: Wed May 17 11:20:02 2023, max compression
```

## Comparing `asimtote-0.16.6.tar` & `asimtote-0.16.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:16:03.085910 asimtote-0.16.6/
--rw-r--r--   0 rcf34      (503) staff       (20)     1334 2023-02-01 17:57:38.000000 asimtote-0.16.6/.gitignore
--rw-r--r--   0 rcf34      (503) staff       (20)     1101 2023-02-01 17:57:38.000000 asimtote-0.16.6/LICENSE
--rw-r--r--   0 rcf34      (503) staff       (20)      297 2023-04-14 17:08:48.000000 asimtote-0.16.6/Makefile
--rw-r--r--   0 rcf34      (503) staff       (20)     3483 2023-04-17 14:16:03.085778 asimtote-0.16.6/PKG-INFO
--rw-r--r--   0 rcf34      (503) staff       (20)     3016 2023-04-14 17:08:48.000000 asimtote-0.16.6/README.md
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:16:03.079585 asimtote-0.16.6/asimtote/
--rw-r--r--   0 rcf34      (503) staff       (20)       45 2023-04-17 14:15:37.000000 asimtote-0.16.6/asimtote/__init__.py
--rw-r--r--   0 rcf34      (503) staff       (20)    13909 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/__main__.py
--rw-r--r--   0 rcf34      (503) staff       (20)    16544 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/config.py
--rw-r--r--   0 rcf34      (503) staff       (20)    74793 2023-04-17 14:15:37.000000 asimtote-0.16.6/asimtote/diff.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:16:03.081388 asimtote-0.16.6/asimtote/ios/
--rw-r--r--   0 rcf34      (503) staff       (20)      188 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/ios/__init__.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:16:03.082221 asimtote-0.16.6/asimtote/ios/commands/
--rw-r--r--   0 rcf34      (503) staff       (20)      719 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/ios/commands/__init__.py
--rw-r--r--   0 rcf34      (503) staff       (20)    18303 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/ios/commands/interface.py
--rw-r--r--   0 rcf34      (503) staff       (20)     5931 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/ios/commands/lists.py
--rw-r--r--   0 rcf34      (503) staff       (20)     8074 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/ios/commands/other.py
--rw-r--r--   0 rcf34      (503) staff       (20)    26719 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/ios/commands/router.py
--rw-r--r--   0 rcf34      (503) staff       (20)     6134 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/ios/config.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:16:03.082970 asimtote-0.16.6/asimtote/ios/converters/
--rw-r--r--   0 rcf34      (503) staff       (20)      733 2023-04-17 14:15:37.000000 asimtote-0.16.6/asimtote/ios/converters/__init__.py
--rw-r--r--   0 rcf34      (503) staff       (20)    28322 2023-04-17 14:15:37.000000 asimtote-0.16.6/asimtote/ios/converters/interface.py
--rw-r--r--   0 rcf34      (503) staff       (20)     3441 2023-04-17 14:15:37.000000 asimtote-0.16.6/asimtote/ios/converters/lists.py
--rw-r--r--   0 rcf34      (503) staff       (20)     7726 2023-04-17 14:15:37.000000 asimtote-0.16.6/asimtote/ios/converters/other.py
--rw-r--r--   0 rcf34      (503) staff       (20)    41819 2023-04-17 14:15:37.000000 asimtote-0.16.6/asimtote/ios/converters/router.py
--rw-r--r--   0 rcf34      (503) staff       (20)     4753 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/ios/diff.py
--rw-r--r--   0 rcf34      (503) staff       (20)    22009 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/ios/utils.py
--rw-r--r--   0 rcf34      (503) staff       (20)     1492 2023-04-14 17:08:48.000000 asimtote-0.16.6/asimtote/misc.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:16:03.080411 asimtote-0.16.6/asimtote.egg-info/
--rw-r--r--   0 rcf34      (503) staff       (20)     3483 2023-04-17 14:16:03.000000 asimtote-0.16.6/asimtote.egg-info/PKG-INFO
--rw-r--r--   0 rcf34      (503) staff       (20)     1230 2023-04-17 14:16:03.000000 asimtote-0.16.6/asimtote.egg-info/SOURCES.txt
--rw-r--r--   0 rcf34      (503) staff       (20)        1 2023-04-17 14:16:03.000000 asimtote-0.16.6/asimtote.egg-info/dependency_links.txt
--rw-r--r--   0 rcf34      (503) staff       (20)       23 2023-04-17 14:16:03.000000 asimtote-0.16.6/asimtote.egg-info/requires.txt
--rw-r--r--   0 rcf34      (503) staff       (20)        9 2023-04-17 14:16:03.000000 asimtote-0.16.6/asimtote.egg-info/top_level.txt
--rw-r--r--   0 rcf34      (503) staff       (20)       38 2023-04-17 14:16:03.085945 asimtote-0.16.6/setup.cfg
--rwxr-xr-x   0 rcf34      (503) staff       (20)      807 2023-04-14 17:08:48.000000 asimtote-0.16.6/setup.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:16:03.083166 asimtote-0.16.6/test_asimtote/
--rw-r--r--   0 rcf34      (503) staff       (20)      149 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/__main__.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:16:03.083425 asimtote-0.16.6/test_asimtote/ios/
--rw-r--r--   0 rcf34      (503) staff       (20)      143 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/__init__.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:16:03.084262 asimtote-0.16.6/test_asimtote/ios/config/
--rw-r--r--   0 rcf34      (503) staff       (20)      328 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/config/__init__.py
--rw-r--r--   0 rcf34      (503) staff       (20)    34207 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/config/interface.py
--rw-r--r--   0 rcf34      (503) staff       (20)    14804 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/config/lists.py
--rw-r--r--   0 rcf34      (503) staff       (20)     9991 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/config/other.py
--rw-r--r--   0 rcf34      (503) staff       (20)    60416 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/config/router.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-17 14:16:03.085299 asimtote-0.16.6/test_asimtote/ios/converters/
--rw-r--r--   0 rcf34      (503) staff       (20)      336 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/converters/__init__.py
--rw-r--r--   0 rcf34      (503) staff       (20)     2646 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/converters/cvtunittest.py
--rw-r--r--   0 rcf34      (503) staff       (20)    95324 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/converters/interface.py
--rw-r--r--   0 rcf34      (503) staff       (20)    13090 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/converters/lists.py
--rw-r--r--   0 rcf34      (503) staff       (20)    24061 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/converters/other.py
--rw-r--r--   0 rcf34      (503) staff       (20)   152946 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/converters/router.py
--rw-r--r--   0 rcf34      (503) staff       (20)     2220 2023-04-14 17:08:48.000000 asimtote-0.16.6/test_asimtote/ios/utils.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-05-17 11:20:02.643934 asimtote-0.16.7/
+-rw-r--r--   0 rcf34      (503) staff       (20)     1334 2023-02-01 17:57:38.000000 asimtote-0.16.7/.gitignore
+-rw-r--r--   0 rcf34      (503) staff       (20)     1101 2023-02-01 17:57:38.000000 asimtote-0.16.7/LICENSE
+-rw-r--r--   0 rcf34      (503) staff       (20)      297 2023-05-15 15:10:38.000000 asimtote-0.16.7/Makefile
+-rw-r--r--   0 rcf34      (503) staff       (20)     3483 2023-05-17 11:20:02.643808 asimtote-0.16.7/PKG-INFO
+-rw-r--r--   0 rcf34      (503) staff       (20)     3016 2023-05-15 15:10:38.000000 asimtote-0.16.7/README.md
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-05-17 11:20:02.639228 asimtote-0.16.7/asimtote/
+-rw-r--r--   0 rcf34      (503) staff       (20)       45 2023-05-17 11:18:18.000000 asimtote-0.16.7/asimtote/__init__.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    13909 2023-05-15 15:10:38.000000 asimtote-0.16.7/asimtote/__main__.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    16544 2023-05-15 15:10:38.000000 asimtote-0.16.7/asimtote/config.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    74825 2023-05-15 15:10:38.000000 asimtote-0.16.7/asimtote/diff.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-05-17 11:20:02.640395 asimtote-0.16.7/asimtote/ios/
+-rw-r--r--   0 rcf34      (503) staff       (20)      188 2023-05-15 15:10:38.000000 asimtote-0.16.7/asimtote/ios/__init__.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-05-17 11:20:02.641022 asimtote-0.16.7/asimtote/ios/commands/
+-rw-r--r--   0 rcf34      (503) staff       (20)      719 2023-05-15 15:10:38.000000 asimtote-0.16.7/asimtote/ios/commands/__init__.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    18303 2023-05-15 15:10:38.000000 asimtote-0.16.7/asimtote/ios/commands/interface.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     5931 2023-05-15 15:10:38.000000 asimtote-0.16.7/asimtote/ios/commands/lists.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     8074 2023-05-15 15:10:38.000000 asimtote-0.16.7/asimtote/ios/commands/other.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    26719 2023-05-15 15:10:38.000000 asimtote-0.16.7/asimtote/ios/commands/router.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     6134 2023-05-15 15:10:38.000000 asimtote-0.16.7/asimtote/ios/config.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-05-17 11:20:02.641567 asimtote-0.16.7/asimtote/ios/converters/
+-rw-r--r--   0 rcf34      (503) staff       (20)      733 2023-05-15 15:10:38.000000 asimtote-0.16.7/asimtote/ios/converters/__init__.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    28322 2023-05-15 15:10:38.000000 asimtote-0.16.7/asimtote/ios/converters/interface.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     3441 2023-05-15 15:10:38.000000 asimtote-0.16.7/asimtote/ios/converters/lists.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     7726 2023-05-15 15:10:38.000000 asimtote-0.16.7/asimtote/ios/converters/other.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    41819 2023-05-15 15:10:38.000000 asimtote-0.16.7/asimtote/ios/converters/router.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     4753 2023-05-15 15:10:38.000000 asimtote-0.16.7/asimtote/ios/diff.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    22009 2023-05-15 15:10:38.000000 asimtote-0.16.7/asimtote/ios/utils.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     1492 2023-05-15 15:10:38.000000 asimtote-0.16.7/asimtote/misc.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-05-17 11:20:02.639907 asimtote-0.16.7/asimtote.egg-info/
+-rw-r--r--   0 rcf34      (503) staff       (20)     3483 2023-05-17 11:20:02.000000 asimtote-0.16.7/asimtote.egg-info/PKG-INFO
+-rw-r--r--   0 rcf34      (503) staff       (20)     1230 2023-05-17 11:20:02.000000 asimtote-0.16.7/asimtote.egg-info/SOURCES.txt
+-rw-r--r--   0 rcf34      (503) staff       (20)        1 2023-05-17 11:20:02.000000 asimtote-0.16.7/asimtote.egg-info/dependency_links.txt
+-rw-r--r--   0 rcf34      (503) staff       (20)       21 2023-05-17 11:20:02.000000 asimtote-0.16.7/asimtote.egg-info/requires.txt
+-rw-r--r--   0 rcf34      (503) staff       (20)        9 2023-05-17 11:20:02.000000 asimtote-0.16.7/asimtote.egg-info/top_level.txt
+-rw-r--r--   0 rcf34      (503) staff       (20)       38 2023-05-17 11:20:02.643970 asimtote-0.16.7/setup.cfg
+-rwxr-xr-x   0 rcf34      (503) staff       (20)      805 2023-05-17 11:15:14.000000 asimtote-0.16.7/setup.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-05-17 11:20:02.641688 asimtote-0.16.7/test_asimtote/
+-rw-r--r--   0 rcf34      (503) staff       (20)      149 2023-05-15 15:10:38.000000 asimtote-0.16.7/test_asimtote/__main__.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-05-17 11:20:02.641901 asimtote-0.16.7/test_asimtote/ios/
+-rw-r--r--   0 rcf34      (503) staff       (20)      143 2023-05-15 15:10:38.000000 asimtote-0.16.7/test_asimtote/ios/__init__.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-05-17 11:20:02.642811 asimtote-0.16.7/test_asimtote/ios/config/
+-rw-r--r--   0 rcf34      (503) staff       (20)      328 2023-05-15 15:10:38.000000 asimtote-0.16.7/test_asimtote/ios/config/__init__.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    34207 2023-05-15 15:10:38.000000 asimtote-0.16.7/test_asimtote/ios/config/interface.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    14804 2023-05-15 15:10:38.000000 asimtote-0.16.7/test_asimtote/ios/config/lists.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     9991 2023-05-15 15:10:38.000000 asimtote-0.16.7/test_asimtote/ios/config/other.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    60416 2023-05-15 15:10:38.000000 asimtote-0.16.7/test_asimtote/ios/config/router.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-05-17 11:20:02.643567 asimtote-0.16.7/test_asimtote/ios/converters/
+-rw-r--r--   0 rcf34      (503) staff       (20)      336 2023-05-15 15:10:38.000000 asimtote-0.16.7/test_asimtote/ios/converters/__init__.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     2646 2023-05-15 15:10:38.000000 asimtote-0.16.7/test_asimtote/ios/converters/cvtunittest.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    95324 2023-05-15 15:10:38.000000 asimtote-0.16.7/test_asimtote/ios/converters/interface.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    13090 2023-05-15 15:10:38.000000 asimtote-0.16.7/test_asimtote/ios/converters/lists.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    24061 2023-05-15 15:10:38.000000 asimtote-0.16.7/test_asimtote/ios/converters/other.py
+-rw-r--r--   0 rcf34      (503) staff       (20)   152946 2023-05-15 15:10:38.000000 asimtote-0.16.7/test_asimtote/ios/converters/router.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     2220 2023-05-15 15:10:38.000000 asimtote-0.16.7/test_asimtote/ios/utils.py
```

### Comparing `asimtote-0.16.6/.gitignore` & `asimtote-0.16.7/.gitignore`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/LICENSE` & `asimtote-0.16.7/LICENSE`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/PKG-INFO` & `asimtote-0.16.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asimtote
-Version: 0.16.6
+Version: 0.16.7
 Summary: Compare network device configuration files using contextual structures
 Home-page: https://gitlab.developers.cam.ac.uk/uis/netsys/udn/asimtote
 Author: Robert Franklin
 Author-email: rcf34@cam.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `asimtote-0.16.6/README.md` & `asimtote-0.16.7/README.md`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/asimtote/__main__.py` & `asimtote-0.16.7/asimtote/__main__.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/asimtote/config.py` & `asimtote-0.16.7/asimtote/config.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/asimtote/diff.py` & `asimtote-0.16.7/asimtote/diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -1457,15 +1457,15 @@
                         remove_is_truncate = True
 
 
                     if self._debug_convert >= DEBUG_CONVERT_MATCH:
                         debug_msg.append(
                             "=> "
                             + ("truncate" if remove_is_truncate else "remove")
-                            + " match: "
+                            + ": "
                             + pathstr(match, cvt.wildcard_indices))
 
 
                     # get elements in the path matching wildcards
 
                     context_args, local_args = cvt.get_args(match)
 
@@ -1666,15 +1666,15 @@
                         update_is_add = True
 
 
                     if self._debug_convert >= DEBUG_CONVERT_MATCH:
                         debug_msg.append(
                             "=> "
                             + ("add" if update_is_add else "update")
-                            + " match: "
+                            + ": "
                             + pathstr(match, cvt.wildcard_indices))
 
 
                     # (same as in remove, above)
 
                     context_args, local_args = cvt.get_args(match)
 
@@ -1813,17 +1813,19 @@
                     and (match not in remove_matches)
                     and (match not in update_matches)):
 
                     debug_msg = []
 
                     if self._debug_convert >= DEBUG_CONVERT_MATCH:
                         debug_msg.append(
-                            "=> trigger match: %s @ %s"
-                                % (cvt.block,
-                                   pathstr(match, cvt.wildcard_indices)))
+                            "=> trigger: "
+                            + pathstr(match, cvt.wildcard_indices)
+                            + " ["
+                            + cvt.block
+                            + "]")
 
 
                     # (same as in remove, above)
 
                     context_args, local_args = cvt.get_args(match)
 
                     try:
```

### Comparing `asimtote-0.16.6/asimtote/ios/commands/__init__.py` & `asimtote-0.16.7/asimtote/ios/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/asimtote/ios/commands/interface.py` & `asimtote-0.16.7/asimtote/ios/commands/interface.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/asimtote/ios/commands/lists.py` & `asimtote-0.16.7/asimtote/ios/commands/lists.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/asimtote/ios/commands/other.py` & `asimtote-0.16.7/asimtote/ios/commands/other.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/asimtote/ios/commands/router.py` & `asimtote-0.16.7/asimtote/ios/commands/router.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/asimtote/ios/config.py` & `asimtote-0.16.7/asimtote/ios/config.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/asimtote/ios/converters/__init__.py` & `asimtote-0.16.7/asimtote/ios/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/asimtote/ios/converters/interface.py` & `asimtote-0.16.7/asimtote/ios/converters/interface.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/asimtote/ios/converters/lists.py` & `asimtote-0.16.7/asimtote/ios/converters/lists.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/asimtote/ios/converters/other.py` & `asimtote-0.16.7/asimtote/ios/converters/other.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/asimtote/ios/converters/router.py` & `asimtote-0.16.7/asimtote/ios/converters/router.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/asimtote/ios/diff.py` & `asimtote-0.16.7/asimtote/ios/diff.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/asimtote/ios/utils.py` & `asimtote-0.16.7/asimtote/ios/utils.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/asimtote/misc.py` & `asimtote-0.16.7/asimtote/misc.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/asimtote.egg-info/PKG-INFO` & `asimtote-0.16.7/asimtote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asimtote
-Version: 0.16.6
+Version: 0.16.7
 Summary: Compare network device configuration files using contextual structures
 Home-page: https://gitlab.developers.cam.ac.uk/uis/netsys/udn/asimtote
 Author: Robert Franklin
 Author-email: rcf34@cam.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `asimtote-0.16.6/asimtote.egg-info/SOURCES.txt` & `asimtote-0.16.7/asimtote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/setup.py` & `asimtote-0.16.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     author_email="rcf34@cam.ac.uk",
     description="Compare network device configuration files using contextual structures",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.developers.cam.ac.uk/uis/netsys/udn/asimtote",
     packages=setuptools.find_packages(),
     install_requires=[
-        "deepops>=1.7.1",
+        "deepops>=1.8",
         "netaddr",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

### Comparing `asimtote-0.16.6/test_asimtote/ios/config/interface.py` & `asimtote-0.16.7/test_asimtote/ios/config/interface.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/test_asimtote/ios/config/lists.py` & `asimtote-0.16.7/test_asimtote/ios/config/lists.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/test_asimtote/ios/config/other.py` & `asimtote-0.16.7/test_asimtote/ios/config/other.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/test_asimtote/ios/config/router.py` & `asimtote-0.16.7/test_asimtote/ios/config/router.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/test_asimtote/ios/converters/cvtunittest.py` & `asimtote-0.16.7/test_asimtote/ios/converters/cvtunittest.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/test_asimtote/ios/converters/interface.py` & `asimtote-0.16.7/test_asimtote/ios/converters/interface.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/test_asimtote/ios/converters/lists.py` & `asimtote-0.16.7/test_asimtote/ios/converters/lists.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/test_asimtote/ios/converters/other.py` & `asimtote-0.16.7/test_asimtote/ios/converters/other.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/test_asimtote/ios/converters/router.py` & `asimtote-0.16.7/test_asimtote/ios/converters/router.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.6/test_asimtote/ios/utils.py` & `asimtote-0.16.7/test_asimtote/ios/utils.py`

 * *Files identical despite different names*

