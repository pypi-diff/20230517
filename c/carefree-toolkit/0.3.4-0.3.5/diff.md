# Comparing `tmp/carefree-toolkit-0.3.4.tar.gz` & `tmp/carefree-toolkit-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-toolkit-0.3.4.tar", last modified: Wed Mar 29 07:18:17 2023, max compression
+gzip compressed data, was "carefree-toolkit-0.3.5.tar", last modified: Wed May 17 13:18:05 2023, max compression
```

## Comparing `carefree-toolkit-0.3.4.tar` & `carefree-toolkit-0.3.5.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 07:18:17.911679 carefree-toolkit-0.3.4/
--rw-rw-rw-   0        0        0     1090 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.4/LICENSE
--rw-rw-rw-   0        0        0     9006 2023-03-29 07:18:17.911679 carefree-toolkit-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     8579 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-29 07:18:17.905679 carefree-toolkit-0.3.4/carefree_toolkit.egg-info/
--rw-rw-rw-   0        0        0     9006 2023-03-29 07:18:17.000000 carefree-toolkit-0.3.4/carefree_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      404 2023-03-29 07:18:17.000000 carefree-toolkit-0.3.4/carefree_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 07:18:17.000000 carefree-toolkit-0.3.4/carefree_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-03-29 07:18:17.000000 carefree-toolkit-0.3.4/carefree_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-29 07:18:17.000000 carefree-toolkit-0.3.4/carefree_toolkit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-29 07:18:17.910679 carefree-toolkit-0.3.4/cftool/
--rw-rw-rw-   0        0        0        0 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.4/cftool/__init__.py
--rw-rw-rw-   0        0        0    22677 2023-03-28 02:09:10.000000 carefree-toolkit-0.3.4/cftool/array.py
--rw-rw-rw-   0        0        0       38 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.4/cftool/constants.py
--rw-rw-rw-   0        0        0     8445 2023-03-28 02:09:18.000000 carefree-toolkit-0.3.4/cftool/cv.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:18:17.910679 carefree-toolkit-0.3.4/cftool/dist/
--rw-rw-rw-   0        0        0       28 2023-03-05 03:09:06.000000 carefree-toolkit-0.3.4/cftool/dist/__init__.py
--rw-rw-rw-   0        0        0    21842 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.4/cftool/dist/core.py
--rw-rw-rw-   0        0        0    25320 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.4/cftool/manage.py
--rw-rw-rw-   0        0        0    84970 2023-03-29 05:19:37.000000 carefree-toolkit-0.3.4/cftool/misc.py
--rw-rw-rw-   0        0        0     6451 2023-03-21 11:08:09.000000 carefree-toolkit-0.3.4/cftool/pipeline.py
--rw-rw-rw-   0        0        0     1004 2023-03-28 02:09:02.000000 carefree-toolkit-0.3.4/cftool/types.py
--rw-rw-rw-   0        0        0       42 2023-03-29 07:18:17.911679 carefree-toolkit-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      886 2023-03-29 07:17:55.000000 carefree-toolkit-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:18:05.334474 carefree-toolkit-0.3.5/
+-rw-rw-rw-   0        0        0     1090 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0     9006 2023-05-17 13:18:05.334474 carefree-toolkit-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8579 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 13:18:05.328497 carefree-toolkit-0.3.5/carefree_toolkit.egg-info/
+-rw-rw-rw-   0        0        0     9006 2023-05-17 13:18:05.000000 carefree-toolkit-0.3.5/carefree_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2023-05-17 13:18:05.000000 carefree-toolkit-0.3.5/carefree_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 13:18:05.000000 carefree-toolkit-0.3.5/carefree_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-17 13:18:05.000000 carefree-toolkit-0.3.5/carefree_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-17 13:18:05.000000 carefree-toolkit-0.3.5/carefree_toolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 13:18:05.333478 carefree-toolkit-0.3.5/cftool/
+-rw-rw-rw-   0        0        0        0 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.5/cftool/__init__.py
+-rw-rw-rw-   0        0        0    22677 2023-03-28 02:09:10.000000 carefree-toolkit-0.3.5/cftool/array.py
+-rw-rw-rw-   0        0        0       58 2023-05-17 12:47:47.000000 carefree-toolkit-0.3.5/cftool/constants.py
+-rw-rw-rw-   0        0        0     8445 2023-03-28 02:09:18.000000 carefree-toolkit-0.3.5/cftool/cv.py
+-rw-rw-rw-   0        0        0     9069 2023-05-17 13:13:34.000000 carefree-toolkit-0.3.5/cftool/data_structures.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:18:05.333478 carefree-toolkit-0.3.5/cftool/dist/
+-rw-rw-rw-   0        0        0       28 2023-03-05 03:09:06.000000 carefree-toolkit-0.3.5/cftool/dist/__init__.py
+-rw-rw-rw-   0        0        0    21842 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.5/cftool/dist/core.py
+-rw-rw-rw-   0        0        0    25320 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.5/cftool/manage.py
+-rw-rw-rw-   0        0        0    85083 2023-05-17 12:43:37.000000 carefree-toolkit-0.3.5/cftool/misc.py
+-rw-rw-rw-   0        0        0     6451 2023-03-21 11:08:09.000000 carefree-toolkit-0.3.5/cftool/pipeline.py
+-rw-rw-rw-   0        0        0     1004 2023-03-28 02:09:02.000000 carefree-toolkit-0.3.5/cftool/types.py
+-rw-rw-rw-   0        0        0     2237 2023-05-17 12:54:11.000000 carefree-toolkit-0.3.5/cftool/web.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 13:18:05.334474 carefree-toolkit-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      886 2023-05-17 13:05:32.000000 carefree-toolkit-0.3.5/setup.py
```

### Comparing `carefree-toolkit-0.3.4/LICENSE` & `carefree-toolkit-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.4/PKG-INFO` & `carefree-toolkit-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: carefree-toolkit
-Version: 0.3.4
+Version: 0.3.5
 Summary: Some commonly used functions and modules
 Home-page: https://github.com/carefree0910/carefree-toolkit
-Download-URL: https://github.com/carefree0910/carefree-toolkit/archive/v0.3.4.tar.gz
+Download-URL: https://github.com/carefree0910/carefree-toolkit/archive/v0.3.5.tar.gz
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python numpy data-science
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # carefree-toolkit
```

### Comparing `carefree-toolkit-0.3.4/README.md` & `carefree-toolkit-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.4/carefree_toolkit.egg-info/PKG-INFO` & `carefree-toolkit-0.3.5/carefree_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: carefree-toolkit
-Version: 0.3.4
+Version: 0.3.5
 Summary: Some commonly used functions and modules
 Home-page: https://github.com/carefree0910/carefree-toolkit
-Download-URL: https://github.com/carefree0910/carefree-toolkit/archive/v0.3.4.tar.gz
+Download-URL: https://github.com/carefree0910/carefree-toolkit/archive/v0.3.5.tar.gz
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python numpy data-science
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # carefree-toolkit
```

### Comparing `carefree-toolkit-0.3.4/cftool/array.py` & `carefree-toolkit-0.3.5/cftool/array.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.4/cftool/cv.py` & `carefree-toolkit-0.3.5/cftool/cv.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.4/cftool/dist/core.py` & `carefree-toolkit-0.3.5/cftool/dist/core.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.4/cftool/manage.py` & `carefree-toolkit-0.3.5/cftool/manage.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.4/cftool/misc.py` & `carefree-toolkit-0.3.5/cftool/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -479,14 +479,18 @@
             return fn(*new_args, **new_kwargs)
 
         return inner
 
     return wrapper
 
 
+def get_err_msg(err: Exception) -> str:
+    return " | ".join(map(repr, sys.exc_info()[:2] + (str(err),)))
+
+
 # util modules
 
 
 TRegister = TypeVar("TRegister", bound="WithRegister", covariant=True)
 TSerializable = TypeVar("TSerializable", bound="ISerializable", covariant=True)
 TSerializableArrays = TypeVar(
     "TSerializableArrays",
```

### Comparing `carefree-toolkit-0.3.4/cftool/pipeline.py` & `carefree-toolkit-0.3.5/cftool/pipeline.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.4/cftool/types.py` & `carefree-toolkit-0.3.5/cftool/types.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.4/setup.py` & `carefree-toolkit-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = "0.3.4"
+VERSION = "0.3.5"
 
 DESCRIPTION = "Some commonly used functions and modules"
 with open("README.md") as f:
     LONG_DESCRIPTION = f.read()
 
 INSTALL_REQUIRES = [
     "dill",
```

