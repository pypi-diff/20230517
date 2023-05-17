# Comparing `tmp/relative-addons-system-2.5.0.tar.gz` & `tmp/relative-addons-system-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relative-addons-system-2.5.0.tar", last modified: Tue May  2 09:09:09 2023, max compression
+gzip compressed data, was "relative-addons-system-2.5.1.tar", last modified: Wed May 17 18:49:53 2023, max compression
```

## Comparing `relative-addons-system-2.5.0.tar` & `relative-addons-system-2.5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 09:09:09.089102 relative-addons-system-2.5.0/
--rw-rw-rw-   0        0        0     1064 2022-10-11 13:46:50.000000 relative-addons-system-2.5.0/LICENSE
--rw-rw-rw-   0        0        0     5784 2023-05-02 09:09:09.086102 relative-addons-system-2.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3851 2023-05-02 08:59:29.000000 relative-addons-system-2.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 09:09:09.017121 relative-addons-system-2.5.0/RelativeAddonsSystem/
--rw-rw-rw-   0        0        0      309 2023-05-02 09:00:55.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:09:09.026101 relative-addons-system-2.5.0/RelativeAddonsSystem/addon/
--rw-rw-rw-   0        0        0     5402 2023-05-02 08:41:08.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/addon/__init__.py
--rw-rw-rw-   0        0        0     1632 2023-05-02 08:26:45.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/addon/metadata.py
--rw-rw-rw-   0        0        0     1911 2023-05-02 08:06:08.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/libraries.py
--rw-rw-rw-   0        0        0    10612 2023-05-02 08:38:57.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/system.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:09:09.052100 relative-addons-system-2.5.0/RelativeAddonsSystem/utils/
--rw-rw-rw-   0        0        0      215 2023-04-16 16:56:05.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/utils/__init__.py
--rw-rw-rw-   0        0        0     2466 2023-05-02 08:33:45.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/utils/cache.py
--rw-rw-rw-   0        0        0      382 2022-10-25 18:37:38.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/utils/recursive_reload_module.py
--rw-rw-rw-   0        0        0     1629 2023-05-02 08:40:18.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/utils/storage.py
--rw-rw-rw-   0        0        0     1442 2022-05-31 14:24:28.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/utils/version_checker.py
--rw-rw-rw-   0        0        0      397 2023-05-02 08:06:08.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/utils/version_transform.py
--rw-rw-rw-   0        0        0      760 2023-05-02 09:02:47.000000 relative-addons-system-2.5.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-02 09:09:09.083100 relative-addons-system-2.5.0/relative_addons_system.egg-info/
--rw-rw-rw-   0        0        0     5784 2023-05-02 09:09:08.000000 relative-addons-system-2.5.0/relative_addons_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2023-05-02 09:09:08.000000 relative-addons-system-2.5.0/relative_addons_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 09:09:08.000000 relative-addons-system-2.5.0/relative_addons_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 09:09:08.000000 relative-addons-system-2.5.0/relative_addons_system.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-02 09:09:08.000000 relative-addons-system-2.5.0/relative_addons_system.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 09:09:09.089102 relative-addons-system-2.5.0/setup.cfg
--rw-rw-rw-   0        0        0      902 2022-11-08 14:20:04.000000 relative-addons-system-2.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 18:49:53.502823 relative-addons-system-2.5.1/
+-rw-rw-rw-   0        0        0     1064 2022-10-11 13:46:50.000000 relative-addons-system-2.5.1/LICENSE
+-rw-rw-rw-   0        0        0     5788 2023-05-17 18:49:53.500800 relative-addons-system-2.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3851 2023-05-02 08:59:29.000000 relative-addons-system-2.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 18:49:53.469799 relative-addons-system-2.5.1/RelativeAddonsSystem/
+-rw-rw-rw-   0        0        0      309 2023-05-17 18:40:17.000000 relative-addons-system-2.5.1/RelativeAddonsSystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 18:49:53.473797 relative-addons-system-2.5.1/RelativeAddonsSystem/addon/
+-rw-rw-rw-   0        0        0     5402 2023-05-02 08:41:08.000000 relative-addons-system-2.5.1/RelativeAddonsSystem/addon/__init__.py
+-rw-rw-rw-   0        0        0     1632 2023-05-02 08:26:45.000000 relative-addons-system-2.5.1/RelativeAddonsSystem/addon/metadata.py
+-rw-rw-rw-   0        0        0     1999 2023-05-17 18:40:17.000000 relative-addons-system-2.5.1/RelativeAddonsSystem/libraries.py
+-rw-rw-rw-   0        0        0    10612 2023-05-02 08:38:57.000000 relative-addons-system-2.5.1/RelativeAddonsSystem/system.py
+drwxrwxrwx   0        0        0        0 2023-05-17 18:49:53.486802 relative-addons-system-2.5.1/RelativeAddonsSystem/utils/
+-rw-rw-rw-   0        0        0      215 2023-04-16 16:56:05.000000 relative-addons-system-2.5.1/RelativeAddonsSystem/utils/__init__.py
+-rw-rw-rw-   0        0        0     2466 2023-05-02 08:33:45.000000 relative-addons-system-2.5.1/RelativeAddonsSystem/utils/cache.py
+-rw-rw-rw-   0        0        0      382 2022-10-25 18:37:38.000000 relative-addons-system-2.5.1/RelativeAddonsSystem/utils/recursive_reload_module.py
+-rw-rw-rw-   0        0        0     1629 2023-05-02 08:40:18.000000 relative-addons-system-2.5.1/RelativeAddonsSystem/utils/storage.py
+-rw-rw-rw-   0        0        0     1442 2022-05-31 14:24:28.000000 relative-addons-system-2.5.1/RelativeAddonsSystem/utils/version_checker.py
+-rw-rw-rw-   0        0        0      397 2023-05-02 08:06:08.000000 relative-addons-system-2.5.1/RelativeAddonsSystem/utils/version_transform.py
+-rw-rw-rw-   0        0        0      764 2023-05-17 18:44:41.000000 relative-addons-system-2.5.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-17 18:49:53.498800 relative-addons-system-2.5.1/relative_addons_system.egg-info/
+-rw-rw-rw-   0        0        0     5788 2023-05-17 18:49:53.000000 relative-addons-system-2.5.1/relative_addons_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2023-05-17 18:49:53.000000 relative-addons-system-2.5.1/relative_addons_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 18:49:53.000000 relative-addons-system-2.5.1/relative_addons_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-17 18:49:53.000000 relative-addons-system-2.5.1/relative_addons_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-17 18:49:53.000000 relative-addons-system-2.5.1/relative_addons_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 18:49:53.502823 relative-addons-system-2.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      902 2022-11-08 14:20:04.000000 relative-addons-system-2.5.1/setup.py
```

### Comparing `relative-addons-system-2.5.0/LICENSE` & `relative-addons-system-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.0/PKG-INFO` & `relative-addons-system-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: relative-addons-system
-Version: 2.5.0
+Version: 2.5.1
 Summary: Easier way to manage your project addons
 Home-page: 
 Author: YoungTitanium
-Author-email: "kuyugama(youngtitanium)" <kuyugamas@gmail.com>
+Author-email: "kuyugama(youngtitanium)" <mail.kuyugama@gmail.com>
 License: Copyright 2022 kuyugama(youngtitanium)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `relative-addons-system-2.5.0/README.md` & `relative-addons-system-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.0/RelativeAddonsSystem/addon/__init__.py` & `relative-addons-system-2.5.1/RelativeAddonsSystem/addon/__init__.py`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.0/RelativeAddonsSystem/addon/metadata.py` & `relative-addons-system-2.5.1/RelativeAddonsSystem/addon/metadata.py`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.0/RelativeAddonsSystem/libraries.py` & `relative-addons-system-2.5.1/RelativeAddonsSystem/libraries.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,16 +20,21 @@
     """
 
     if force or len(installed_libraries.get()) == 0:
         pip_out = subprocess.getoutput(str(pip_executable.absolute()) + " freeze")
 
         libs = {}
 
-        for lib in pip_out.splitlines():
-            name, version = lib.lower().split("==")
+        for lib_line in pip_out.splitlines():
+            lib = lib_line.lower().split("==")
+
+            if len(lib) < 2:
+                continue
+
+            name, version = lib
             libs[name] = version
 
         installed_libraries.set(libs)
 
     return installed_libraries.get()
```

### Comparing `relative-addons-system-2.5.0/RelativeAddonsSystem/system.py` & `relative-addons-system-2.5.1/RelativeAddonsSystem/system.py`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.0/RelativeAddonsSystem/utils/cache.py` & `relative-addons-system-2.5.1/RelativeAddonsSystem/utils/cache.py`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.0/RelativeAddonsSystem/utils/storage.py` & `relative-addons-system-2.5.1/RelativeAddonsSystem/utils/storage.py`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.0/RelativeAddonsSystem/utils/version_checker.py` & `relative-addons-system-2.5.1/RelativeAddonsSystem/utils/version_checker.py`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.0/pyproject.toml` & `relative-addons-system-2.5.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "relative-addons-system"
-version = "2.5.0"
+version = "2.5.1"
 description = "Easier way to manage your project addons"
-authors = [{ name = "kuyugama(youngtitanium)", email = "kuyugamas@gmail.com" }]
+authors = [{ name = "kuyugama(youngtitanium)", email = "mail.kuyugama@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Topic :: Utilities"
 ]
```

### Comparing `relative-addons-system-2.5.0/relative_addons_system.egg-info/PKG-INFO` & `relative-addons-system-2.5.1/relative_addons_system.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: relative-addons-system
-Version: 2.5.0
+Version: 2.5.1
 Summary: Easier way to manage your project addons
 Home-page: 
 Author: YoungTitanium
-Author-email: "kuyugama(youngtitanium)" <kuyugamas@gmail.com>
+Author-email: "kuyugama(youngtitanium)" <mail.kuyugama@gmail.com>
 License: Copyright 2022 kuyugama(youngtitanium)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `relative-addons-system-2.5.0/relative_addons_system.egg-info/SOURCES.txt` & `relative-addons-system-2.5.1/relative_addons_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.0/setup.py` & `relative-addons-system-2.5.1/setup.py`

 * *Files identical despite different names*

