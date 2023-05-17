# Comparing `tmp/qim3d-0.1.0.tar.gz` & `tmp/qim3d-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qim3d-0.1.0.tar", last modified: Wed May 17 12:50:24 2023, max compression
+gzip compressed data, was "qim3d-0.1.1.tar", last modified: Wed May 17 13:13:01 2023, max compression
```

## Comparing `qim3d-0.1.0.tar` & `qim3d-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 fima     (300707) unixusers  (1040)        0 2023-05-17 12:50:24.605721 qim3d-0.1.0/
--rw-r--r--   0 fima     (300707) unixusers  (1040)     1060 2023-05-12 08:06:02.000000 qim3d-0.1.0/LICENSE
--rw-r--r--   0 fima     (300707) unixusers  (1040)     2024 2023-05-17 12:50:24.605721 qim3d-0.1.0/PKG-INFO
--rw-r--r--   0 fima     (300707) unixusers  (1040)     1241 2023-05-17 12:47:28.000000 qim3d-0.1.0/README.md
-drwxr-xr-x   0 fima     (300707) unixusers  (1040)        0 2023-05-17 12:50:24.605721 qim3d-0.1.0/qim3d/
--rw-r--r--   0 fima     (300707) unixusers  (1040)       51 2023-05-17 12:47:26.000000 qim3d-0.1.0/qim3d/__init__.py
-drwxr-xr-x   0 fima     (300707) unixusers  (1040)        0 2023-05-17 12:50:24.605721 qim3d-0.1.0/qim3d/gui/
--rw-r--r--   0 fima     (300707) unixusers  (1040)       77 2023-05-16 10:43:37.000000 qim3d-0.1.0/qim3d/gui/__init__.py
--rw-r--r--   0 fima     (300707) unixusers  (1040)    14577 2023-05-17 12:47:24.000000 qim3d-0.1.0/qim3d/gui/data_explorer.py
--rw-r--r--   0 fima     (300707) unixusers  (1040)    14592 2023-05-17 12:47:23.000000 qim3d-0.1.0/qim3d/gui/iso3d.py
--rw-r--r--   0 fima     (300707) unixusers  (1040)    20216 2023-05-17 12:47:20.000000 qim3d-0.1.0/qim3d/gui/local_thickness.py
-drwxr-xr-x   0 fima     (300707) unixusers  (1040)        0 2023-05-17 12:50:24.605721 qim3d-0.1.0/qim3d/io/
--rw-r--r--   0 fima     (300707) unixusers  (1040)       57 2023-05-16 13:57:35.000000 qim3d-0.1.0/qim3d/io/__init__.py
--rw-r--r--   0 fima     (300707) unixusers  (1040)     1748 2023-05-17 07:29:00.000000 qim3d-0.1.0/qim3d/io/load.py
--rw-r--r--   0 fima     (300707) unixusers  (1040)      232 2023-05-16 14:17:09.000000 qim3d-0.1.0/qim3d/io/save.py
-drwxr-xr-x   0 fima     (300707) unixusers  (1040)        0 2023-05-17 12:50:24.605721 qim3d-0.1.0/qim3d/tools/
--rw-r--r--   0 fima     (300707) unixusers  (1040)        0 2023-05-15 10:32:28.000000 qim3d-0.1.0/qim3d/tools/__init__.py
--rw-r--r--   0 fima     (300707) unixusers  (1040)     1405 2023-05-15 10:44:36.000000 qim3d-0.1.0/qim3d/tools/internal_tools.py
-drwxr-xr-x   0 fima     (300707) unixusers  (1040)        0 2023-05-17 12:50:24.605721 qim3d-0.1.0/qim3d.egg-info/
--rw-r--r--   0 fima     (300707) unixusers  (1040)     2024 2023-05-17 12:50:24.000000 qim3d-0.1.0/qim3d.egg-info/PKG-INFO
--rw-r--r--   0 fima     (300707) unixusers  (1040)      394 2023-05-17 12:50:24.000000 qim3d-0.1.0/qim3d.egg-info/SOURCES.txt
--rw-r--r--   0 fima     (300707) unixusers  (1040)        1 2023-05-17 12:50:24.000000 qim3d-0.1.0/qim3d.egg-info/dependency_links.txt
--rw-r--r--   0 fima     (300707) unixusers  (1040)      169 2023-05-17 12:50:24.000000 qim3d-0.1.0/qim3d.egg-info/requires.txt
--rw-r--r--   0 fima     (300707) unixusers  (1040)        6 2023-05-17 12:50:24.000000 qim3d-0.1.0/qim3d.egg-info/top_level.txt
--rw-r--r--   0 fima     (300707) unixusers  (1040)       38 2023-05-17 12:50:24.605721 qim3d-0.1.0/setup.cfg
--rw-r--r--   0 fima     (300707) unixusers  (1040)     1482 2023-05-17 12:42:18.000000 qim3d-0.1.0/setup.py
+drwxr-xr-x   0 fima     (300707) unixusers  (1040)        0 2023-05-17 13:13:01.742592 qim3d-0.1.1/
+-rw-r--r--   0 fima     (300707) unixusers  (1040)     1060 2023-05-12 08:06:02.000000 qim3d-0.1.1/LICENSE
+-rw-r--r--   0 fima     (300707) unixusers  (1040)     2024 2023-05-17 13:13:01.742592 qim3d-0.1.1/PKG-INFO
+-rw-r--r--   0 fima     (300707) unixusers  (1040)     1241 2023-05-17 12:47:28.000000 qim3d-0.1.1/README.md
+drwxr-xr-x   0 fima     (300707) unixusers  (1040)        0 2023-05-17 13:13:01.742592 qim3d-0.1.1/qim3d/
+-rw-r--r--   0 fima     (300707) unixusers  (1040)       51 2023-05-17 12:47:26.000000 qim3d-0.1.1/qim3d/__init__.py
+drwxr-xr-x   0 fima     (300707) unixusers  (1040)        0 2023-05-17 13:13:01.742592 qim3d-0.1.1/qim3d/gui/
+-rw-r--r--   0 fima     (300707) unixusers  (1040)       77 2023-05-16 10:43:37.000000 qim3d-0.1.1/qim3d/gui/__init__.py
+-rw-r--r--   0 fima     (300707) unixusers  (1040)    14577 2023-05-17 12:47:24.000000 qim3d-0.1.1/qim3d/gui/data_explorer.py
+-rw-r--r--   0 fima     (300707) unixusers  (1040)    14586 2023-05-17 13:10:33.000000 qim3d-0.1.1/qim3d/gui/iso3d.py
+-rw-r--r--   0 fima     (300707) unixusers  (1040)    20210 2023-05-17 13:10:20.000000 qim3d-0.1.1/qim3d/gui/local_thickness.py
+drwxr-xr-x   0 fima     (300707) unixusers  (1040)        0 2023-05-17 13:13:01.742592 qim3d-0.1.1/qim3d/io/
+-rw-r--r--   0 fima     (300707) unixusers  (1040)       57 2023-05-16 13:57:35.000000 qim3d-0.1.1/qim3d/io/__init__.py
+-rw-r--r--   0 fima     (300707) unixusers  (1040)     1748 2023-05-17 07:29:00.000000 qim3d-0.1.1/qim3d/io/load.py
+-rw-r--r--   0 fima     (300707) unixusers  (1040)      232 2023-05-16 14:17:09.000000 qim3d-0.1.1/qim3d/io/save.py
+drwxr-xr-x   0 fima     (300707) unixusers  (1040)        0 2023-05-17 13:13:01.742592 qim3d-0.1.1/qim3d/tools/
+-rw-r--r--   0 fima     (300707) unixusers  (1040)        0 2023-05-15 10:32:28.000000 qim3d-0.1.1/qim3d/tools/__init__.py
+-rw-r--r--   0 fima     (300707) unixusers  (1040)     1405 2023-05-15 10:44:36.000000 qim3d-0.1.1/qim3d/tools/internal_tools.py
+drwxr-xr-x   0 fima     (300707) unixusers  (1040)        0 2023-05-17 13:13:01.742592 qim3d-0.1.1/qim3d.egg-info/
+-rw-r--r--   0 fima     (300707) unixusers  (1040)     2024 2023-05-17 13:13:01.000000 qim3d-0.1.1/qim3d.egg-info/PKG-INFO
+-rw-r--r--   0 fima     (300707) unixusers  (1040)      394 2023-05-17 13:13:01.000000 qim3d-0.1.1/qim3d.egg-info/SOURCES.txt
+-rw-r--r--   0 fima     (300707) unixusers  (1040)        1 2023-05-17 13:13:01.000000 qim3d-0.1.1/qim3d.egg-info/dependency_links.txt
+-rw-r--r--   0 fima     (300707) unixusers  (1040)      169 2023-05-17 13:13:01.000000 qim3d-0.1.1/qim3d.egg-info/requires.txt
+-rw-r--r--   0 fima     (300707) unixusers  (1040)        6 2023-05-17 13:13:01.000000 qim3d-0.1.1/qim3d.egg-info/top_level.txt
+-rw-r--r--   0 fima     (300707) unixusers  (1040)       38 2023-05-17 13:13:01.742592 qim3d-0.1.1/setup.cfg
+-rw-r--r--   0 fima     (300707) unixusers  (1040)     1482 2023-05-17 13:12:19.000000 qim3d-0.1.1/setup.py
```

### Comparing `qim3d-0.1.0/LICENSE` & `qim3d-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qim3d-0.1.0/PKG-INFO` & `qim3d-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qim3d
-Version: 0.1.0
+Version: 0.1.1
 Summary: QIM tools and user interfaces
 Home-page: https://lab.compute.dtu.dk/QIM/qim
 Author: Felipe Delestro
 Author-email: fima@dtu.dk
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
```

### Comparing `qim3d-0.1.0/README.md` & `qim3d-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `qim3d-0.1.0/qim3d/gui/data_explorer.py` & `qim3d-0.1.1/qim3d/gui/data_explorer.py`

 * *Files identical despite different names*

### Comparing `qim3d-0.1.0/qim3d/gui/iso3d.py` & `qim3d-0.1.1/qim3d/gui/iso3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
         self.plot_height = 768
         self.height = 1024
         self.width = 960
 
         # Data examples
         current_dir = os.path.dirname(os.path.abspath(__file__))
-        examples_dir = ["..", "..", "img_examples"]
+        examples_dir = ["..", "img_examples"]
         examples = [
             "blobs_256x256x256.tif",
             "fly_150x256x256.tif",
             "cement_128x128x128.tif",
             "NT_10x200x100.tif",
             "NT_128x128x128.tif",
             "shell_225x128x128.tif",
```

### Comparing `qim3d-0.1.0/qim3d/gui/local_thickness.py` & `qim3d-0.1.1/qim3d/gui/local_thickness.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.title = "Local thickness"
         self.plot_height = 768
         self.height = 1024
         self.width = 960
 
         # Data examples
         current_dir = os.path.dirname(os.path.abspath(__file__))
-        examples_dir = ["..", "..", "img_examples"]
+        examples_dir = ["..", "img_examples"]
         examples = [
             "blobs_256x256x256.tif",
             "cement_128x128x128.tif",
             "bone_128x128x128.tif",
             "NT_10x200x100.tif",
         ]
         self.img_examples = []
```

### Comparing `qim3d-0.1.0/qim3d/io/load.py` & `qim3d-0.1.1/qim3d/io/load.py`

 * *Files identical despite different names*

### Comparing `qim3d-0.1.0/qim3d/tools/internal_tools.py` & `qim3d-0.1.1/qim3d/tools/internal_tools.py`

 * *Files identical despite different names*

### Comparing `qim3d-0.1.0/qim3d.egg-info/PKG-INFO` & `qim3d-0.1.1/qim3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qim3d
-Version: 0.1.0
+Version: 0.1.1
 Summary: QIM tools and user interfaces
 Home-page: https://lab.compute.dtu.dk/QIM/qim
 Author: Felipe Delestro
 Author-email: fima@dtu.dk
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
```

### Comparing `qim3d-0.1.0/setup.py` & `qim3d-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Read the contents of your README file
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="qim3d",
-    version="0.1.0",
+    version="0.1.1",
     author="Felipe Delestro",
     author_email="fima@dtu.dk",
     description="QIM tools and user interfaces",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://lab.compute.dtu.dk/QIM/qim",
     packages=find_packages(),
```

