# Comparing `tmp/xerxes-protocol-1.4.1.tar.gz` & `tmp/xerxes-protocol-1.4.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xerxes-protocol-1.4.1.tar", last modified: Thu Mar  2 15:03:10 2023, max compression
+gzip compressed data, was "xerxes-protocol-1.4.2a1.tar", last modified: Wed May 17 09:52:13 2023, max compression
```

## Comparing `xerxes-protocol-1.4.1.tar` & `xerxes-protocol-1.4.2a1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:03:10.382871 xerxes-protocol-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-03-02 15:03:10.382871 xerxes-protocol-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 15:03:10.382871 xerxes-protocol-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:03:10.378871 xerxes-protocol-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/tests/test_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/tests/test_memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:03:10.378871 xerxes-protocol-1.4.1/xerxes_protocol/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1515 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/cli_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/debug_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/error_flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:03:10.378871 xerxes-protocol-1.4.1/xerxes_protocol/hierarchy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/hierarchy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:03:10.378871 xerxes-protocol-1.4.1/xerxes_protocol/hierarchy/leaves/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/hierarchy/leaves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/hierarchy/leaves/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/hierarchy/leaves/inclination.py
--rw-r--r--   0 runner    (1001) docker     (123)    13664 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/hierarchy/leaves/leaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/hierarchy/leaves/pressure.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/hierarchy/leaves/strain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/hierarchy/leaves/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/hierarchy/root.py
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:03:10.382871 xerxes-protocol-1.4.1/xerxes_protocol/units/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/units/angle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/units/density.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/units/length.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/units/pressure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/units/temp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-02 15:02:58.000000 xerxes-protocol-1.4.1/xerxes_protocol/units/unit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:03:10.378871 xerxes-protocol-1.4.1/xerxes_protocol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-03-02 15:03:10.000000 xerxes-protocol-1.4.1/xerxes_protocol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-02 15:03:10.000000 xerxes-protocol-1.4.1/xerxes_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 15:03:10.000000 xerxes-protocol-1.4.1/xerxes_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-02 15:03:10.000000 xerxes-protocol-1.4.1/xerxes_protocol.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-02 15:03:10.000000 xerxes-protocol-1.4.1/xerxes_protocol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-02 15:03:10.000000 xerxes-protocol-1.4.1/xerxes_protocol.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:52:13.265143 xerxes-protocol-1.4.2a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-17 09:52:13.265143 xerxes-protocol-1.4.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 09:52:13.265143 xerxes-protocol-1.4.2a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:52:13.257144 xerxes-protocol-1.4.2a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/tests/test_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/tests/test_memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:52:13.257144 xerxes-protocol-1.4.2a1/xerxes_protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3140 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/cli_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/debug_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/error_flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:52:13.261144 xerxes-protocol-1.4.2a1/xerxes_protocol/hierarchy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/hierarchy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:52:13.261144 xerxes-protocol-1.4.2a1/xerxes_protocol/hierarchy/leaves/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/hierarchy/leaves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/hierarchy/leaves/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/hierarchy/leaves/inclination.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/hierarchy/leaves/leaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/hierarchy/leaves/pressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/hierarchy/leaves/strain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/hierarchy/leaves/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/hierarchy/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:52:13.265143 xerxes-protocol-1.4.2a1/xerxes_protocol/units/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/units/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/units/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/units/length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/units/pressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/units/temp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-17 09:51:59.000000 xerxes-protocol-1.4.2a1/xerxes_protocol/units/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:52:13.261144 xerxes-protocol-1.4.2a1/xerxes_protocol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-17 09:52:13.000000 xerxes-protocol-1.4.2a1/xerxes_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-17 09:52:13.000000 xerxes-protocol-1.4.2a1/xerxes_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:52:13.000000 xerxes-protocol-1.4.2a1/xerxes_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 09:52:13.000000 xerxes-protocol-1.4.2a1/xerxes_protocol.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-17 09:52:13.000000 xerxes-protocol-1.4.2a1/xerxes_protocol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 09:52:13.000000 xerxes-protocol-1.4.2a1/xerxes_protocol.egg-info/top_level.txt
```

### Comparing `xerxes-protocol-1.4.1/LICENSE` & `xerxes-protocol-1.4.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/PKG-INFO` & `xerxes-protocol-1.4.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xerxes-protocol
-Version: 1.4.1
+Version: 1.4.2a1
 Summary: Python implementation for xerxes-protocol
 Home-page: https://github.com/metrotech-sk/xerxes-protocol
 Author: Stanislav Rubint
 Author-email: Stanislav Rubint <stanislav@rubint.sk>
 License: MIT License
         
         Copyright (c) 2022 metrotech.sk
```

### Comparing `xerxes-protocol-1.4.1/README.md` & `xerxes-protocol-1.4.2a1/README.md`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/pyproject.toml` & `xerxes-protocol-1.4.2a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "xerxes-protocol"
-version = "1.4.1"
+version = "1.4.2a1"
 description = "Python implementation for xerxes-protocol"
 readme = "README.md"
 #requires_python = '>=3.8'
 license = {file = "LICENSE"}
 authors = [
     {name = "Stanislav Rubint", email = "stanislav@rubint.sk"}
 ]
```

### Comparing `xerxes-protocol-1.4.1/setup.py` & `xerxes-protocol-1.4.2a1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="xerxes-protocol",
-    version="1.4.1",
+    version="1.4.2a1",
     author="Stanislav Rubint",
     author_email="stanislav@rubint.sk",
     description="Python implementation for xerxes-protocol",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/metrotech-sk/xerxes-protocol",
     packages=setuptools.find_packages(),
```

### Comparing `xerxes-protocol-1.4.1/tests/conftest.py` & `xerxes-protocol-1.4.2a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/tests/test_ids.py` & `xerxes-protocol-1.4.2a1/tests/test_ids.py`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/tests/test_memory.py` & `xerxes-protocol-1.4.2a1/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol/__init__.py` & `xerxes-protocol-1.4.2a1/xerxes_protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol/debug_serial.py` & `xerxes-protocol-1.4.2a1/xerxes_protocol/debug_serial.py`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol/defaults.py` & `xerxes-protocol-1.4.2a1/xerxes_protocol/defaults.py`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol/hierarchy/leaves/distance.py` & `xerxes-protocol-1.4.2a1/xerxes_protocol/hierarchy/leaves/distance.py`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol/hierarchy/leaves/inclination.py` & `xerxes-protocol-1.4.2a1/xerxes_protocol/hierarchy/leaves/inclination.py`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol/hierarchy/leaves/leaf.py` & `xerxes-protocol-1.4.2a1/xerxes_protocol/hierarchy/leaves/leaf.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,20 +27,20 @@
 
 import struct
 import logging
 _log = logging.getLogger(__name__)
 
 
 __author__ = "theMladyPan"
-__version__ = "1.4.0"
+__version__ = "1.4.2"
 __license__ = "MIT"
 __email__ = "stanislav@rubint.sk"
 __status__ = "Production"
 __package__ = "xerxes_protocol"
-__date__ = "2023-02-22"
+__date__ = "2023-05-15"
 
 __all__ = [
     "LeafConfig",
     "LeafData",
     "Leaf"
 ]
 
@@ -108,15 +108,15 @@
                     d.update({
                         attribute: attr_val.preferred()
                     })
                     
         return d
 
 
-class  Leaf:
+class Leaf:
     """Base class for all leaf classes.
 
     This class is the base class for all leaf classes. It is used to represent
     a leaf in a convenient way.
 
     Args:
         addr (Addr): The address of the leaf.
```

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol/hierarchy/leaves/pressure.py` & `xerxes-protocol-1.4.2a1/xerxes_protocol/hierarchy/leaves/pressure.py`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol/hierarchy/leaves/strain.py` & `xerxes-protocol-1.4.2a1/xerxes_protocol/hierarchy/leaves/strain.py`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol/hierarchy/leaves/utils.py` & `xerxes-protocol-1.4.2a1/xerxes_protocol/hierarchy/leaves/utils.py`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol/hierarchy/root.py` & `xerxes-protocol-1.4.2a1/xerxes_protocol/hierarchy/root.py`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol/ids.py` & `xerxes-protocol-1.4.2a1/xerxes_protocol/ids.py`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol/memory.py` & `xerxes-protocol-1.4.2a1/xerxes_protocol/memory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 from dataclasses import dataclass
-from typing import final
+
+__author__ = "theMladyPan"
+__version__ = "1.4.2"
+__license__ = "MIT"
+__email__ = "stanislav@rubint.sk"
+__status__ = "Production"
+__package__ = "xerxes_protocol"
+__date__ = "2023-05-15"
 
 # non-volatile memory map (persistent)
 # memory offset of the offset of the process values
 GAIN_PV0_OFFSET = 0
 GAIN_PV1_OFFSET = 4
 GAIN_PV2_OFFSET = 8
 GAIN_PV3_OFFSET = 12
@@ -16,14 +23,20 @@
 
 # memory offset of cycle time in microseconds (4 bytes)
 OFFSET_DESIRED_CYCLE_TIME = 32
 
 OFFSET_CONFIG_BITS = 40
 OFFSET_ADDRESS = 44
 
+# configuration values
+CONFIG_VAL0_OFFSET = 48
+CONFIG_VAL1_OFFSET = 52
+CONFIG_VAL2_OFFSET = 56
+CONFIG_VAL3_OFFSET = 60
+
 # Volatile range (not persistent)
 PV0_OFFSET = 256
 PV1_OFFSET = 260
 PV2_OFFSET = 264
 PV3_OFFSET = 268
 
 MEAN_PV0_OFFSET = 272
@@ -47,14 +60,24 @@
 MAX_PV3_OFFSET = 332
 
 DV0_OFFSET = 336
 DV1_OFFSET = 340
 DV2_OFFSET = 344
 DV3_OFFSET = 348
 
+AV0_OFFSET = 352
+AV1_OFFSET = 356
+AV2_OFFSET = 360
+AV3_OFFSET = 364
+
+SV0_OFFSET = 368
+SV1_OFFSET = 372
+SV2_OFFSET = 376
+SV3_OFFSET = 380
+
 MEM_UNLOCKED_OFFSET = 384
 
 # Read only range
 STATUS_OFFSET = 512
 ERROR_OFFSET = 520
 UID_OFFSET = 528
 
@@ -164,40 +187,48 @@
     
     Attributes:
         gain_pv<n>          (float_t):  The gain of the <n>th process value.
         offset_pv<n>        (float_t):  The offset of the <n>th process value.
         desired_cycle_time  (uint32_t): The desired cycle time in microseconds.
         device_address      (uint8_t):  The device address.
         config              (uint8_t):  The configuration bits.
+        config_val<n>       (uint32_t): The <n>th configuration value.
     """
     gain_pv0 = MemoryElement(GAIN_PV0_OFFSET, float_t)
     gain_pv1 = MemoryElement(GAIN_PV1_OFFSET, float_t)
     gain_pv2 = MemoryElement(GAIN_PV2_OFFSET, float_t)
     gain_pv3 = MemoryElement(GAIN_PV3_OFFSET, float_t)
 
     offset_pv0 = MemoryElement(OFFSET_PV0_OFFSET, float_t)
     offset_pv1 = MemoryElement(OFFSET_PV1_OFFSET, float_t)
     offset_pv2 = MemoryElement(OFFSET_PV2_OFFSET, float_t)
     offset_pv3 = MemoryElement(OFFSET_PV3_OFFSET, float_t)
 
     desired_cycle_time_us = MemoryElement(OFFSET_DESIRED_CYCLE_TIME, uint32_t)
     device_address = MemoryElement(OFFSET_ADDRESS, uint8_t)
     device_config = MemoryElement(OFFSET_CONFIG_BITS, uint8_t)
+
+    config_val0 = MemoryElement(CONFIG_VAL0_OFFSET, uint32_t)
+    config_val1 = MemoryElement(CONFIG_VAL1_OFFSET, uint32_t)
+    config_val2 = MemoryElement(CONFIG_VAL2_OFFSET, uint32_t)
+    config_val3 = MemoryElement(CONFIG_VAL3_OFFSET, uint32_t)
     
 
 class MemoryVolatile(XerxesMemoryType):
     """Represents the volatile memory of the Xerxes memory map.
 
     Attributes:
         pv<n>           (float_t):  The <n>th process value.
         mean_pv<n>      (float_t):  The mean of the <n>th process value.
         std_dev_pv<n>   (float_t):  The standard deviation of the <n>th process value.
         min_pv<n>       (float_t):  The minimum of the <n>th process value.
         max_pv<n>       (float_t):  The maximum of the <n>th process value.
         dv<n>           (uint32_t): The <n>th discrete value (0s or 1s), e.g. for digital inputs or outputs.
+        av<n>           (float_t):  The <n>th analog value, e.g. for analog inputs or outputs.
+        sv<n>           (int32_t):  The <n>th signed value, e.g. for counters.
         mem_unlocked    (uint32_t): Whether the protected memory is unlocked for writing.
     """
 
     pv0 = MemoryElement(PV0_OFFSET, float_t)
     pv1 = MemoryElement(PV1_OFFSET, float_t)
     pv2 = MemoryElement(PV2_OFFSET, float_t)
     pv3 = MemoryElement(PV3_OFFSET, float_t)
@@ -218,18 +249,31 @@
     min_pv3 = MemoryElement(MIN_PV3_OFFSET, float_t)
 
     max_pv0 = MemoryElement(MAX_PV0_OFFSET, float_t)
     max_pv1 = MemoryElement(MAX_PV1_OFFSET, float_t)
     max_pv2 = MemoryElement(MAX_PV2_OFFSET, float_t)
     max_pv3 = MemoryElement(MAX_PV3_OFFSET, float_t)
 
-    dv0 = MemoryElement(DV0_OFFSET, uint32_t)
-    dv1 = MemoryElement(DV1_OFFSET, uint32_t)
-    dv2 = MemoryElement(DV2_OFFSET, uint32_t)
-    dv3 = MemoryElement(DV3_OFFSET, uint32_t)
+    # digital values, for example for digital inputs or outputs
+    dv0 = MemoryElement(DV0_OFFSET, uint32_t)  # digital value 1
+    dv1 = MemoryElement(DV1_OFFSET, uint32_t)  # digital value 2
+    dv2 = MemoryElement(DV2_OFFSET, uint32_t)  # digital value 3
+    dv3 = MemoryElement(DV3_OFFSET, uint32_t)  # digital value 4
+
+    # additional analog values, for example for analog inputs or outputs
+    av0 = MemoryElement(AV0_OFFSET, float_t)  # analog value 0
+    av1 = MemoryElement(AV1_OFFSET, float_t)  # analog value 1
+    av2 = MemoryElement(AV2_OFFSET, float_t)  # analog value 2
+    av3 = MemoryElement(AV3_OFFSET, float_t)  # analog value 3
+    
+    # signed values, for example for PID controllers, counters, etc.
+    sv0 = MemoryElement(SV0_OFFSET, int32_t)  # signed value 0
+    sv1 = MemoryElement(SV1_OFFSET, int32_t)  # signed value 1
+    sv2 = MemoryElement(SV2_OFFSET, int32_t)  # signed value 2
+    sv3 = MemoryElement(SV3_OFFSET, int32_t)  # signed value 3
 
     memory_lock = MemoryElement(MEM_UNLOCKED_OFFSET, uint32_t)
 
 
 class MemoryReadOnly(XerxesMemoryType):
     """Represents the read-only memory of the Xerxes memory map.
```

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol/network.py` & `xerxes-protocol-1.4.2a1/xerxes_protocol/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,20 +23,20 @@
     "XerxesPingReply",
     "FutureXerxesNetwork",
     "XerxesNetwork"
 ]
 
 
 __author__ = "theMladyPan"
-__version__ = "1.4.0"
+__version__ = "1.4.2"
 __license__ = "MIT"
 __email__ = "stanislav@rubint.sk"
 __status__ = "Production"
 __package__ = "xerxes_protocol"
-__date__ = "2023-02-22"
+__date__ = "2023-05-15"
 
 
 class ChecksumError(Exception): 
     """Raised when the checksum of a message is invalid."""
 
 
 class MessageIncomplete(Exception): 
@@ -220,15 +220,15 @@
         >>> # read a message
         >>> msg = network.read_msg()
         >>> print(msg)
         XerxesMessage(source=Addr(0x01), destination=Addr(0x00), length=12, message_id=MsgId(0x00), payload=b'\x04\x01\x04', latency=0.015, crc='U')
 
     """
 
-    _ic = 0
+    _ic = 0  # not used yet
     _instances = {}
     _opened = False
 
 
     def __init__(self, port: serial.Serial) -> None:
         assert isinstance(port, serial.Serial)
         self._s = port
@@ -243,19 +243,18 @@
         
         Returns:
             XerxesNetwork: self
         """
         self._s.baudrate = baudrate
         self._s.timeout = timeout
         
-        # reopen the port with new settings
-        self._s.close()
         if not self._s.isOpen():
             self._s.open()
         self._opened = True
+        self._s._reconfigure_port()
 
         return self
      
 
     @property
     def timeout(self) -> float:
         """Timeout for serial port in seconds."""
```

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol/units/angle.py` & `xerxes-protocol-1.4.2a1/xerxes_protocol/units/angle.py`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol/units/density.py` & `xerxes-protocol-1.4.2a1/xerxes_protocol/units/density.py`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol/units/length.py` & `xerxes-protocol-1.4.2a1/xerxes_protocol/units/length.py`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol/units/pressure.py` & `xerxes-protocol-1.4.2a1/xerxes_protocol/units/pressure.py`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol/units/temp.py` & `xerxes-protocol-1.4.2a1/xerxes_protocol/units/temp.py`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol/units/unit.py` & `xerxes-protocol-1.4.2a1/xerxes_protocol/units/unit.py`

 * *Files identical despite different names*

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol.egg-info/PKG-INFO` & `xerxes-protocol-1.4.2a1/xerxes_protocol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xerxes-protocol
-Version: 1.4.1
+Version: 1.4.2a1
 Summary: Python implementation for xerxes-protocol
 Home-page: https://github.com/metrotech-sk/xerxes-protocol
 Author: Stanislav Rubint
 Author-email: Stanislav Rubint <stanislav@rubint.sk>
 License: MIT License
         
         Copyright (c) 2022 metrotech.sk
```

### Comparing `xerxes-protocol-1.4.1/xerxes_protocol.egg-info/SOURCES.txt` & `xerxes-protocol-1.4.2a1/xerxes_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

