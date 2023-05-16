# Comparing `tmp/augratin-23.5.16.tar.gz` & `tmp/augratin-23.5.16.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "augratin-23.5.16.tar", last modified: Tue May 16 19:45:37 2023, max compression
+gzip compressed data, was "augratin-23.5.16.1.tar", last modified: Tue May 16 23:38:19 2023, max compression
```

## Comparing `augratin-23.5.16.tar` & `augratin-23.5.16.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-16 19:45:37.194069 augratin-23.5.16/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-02-19 00:59:20.000000 augratin-23.5.16/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4644 2023-05-16 19:45:37.194069 augratin-23.5.16/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3869 2023-05-16 19:43:59.000000 augratin-23.5.16/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-16 19:45:37.187069 augratin-23.5.16/augratin/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.16/augratin/__init__.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    39551 2023-05-16 19:37:32.000000 augratin-23.5.16/augratin/__main__.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-16 19:45:37.193069 augratin-23.5.16/augratin/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-17 19:16:23.000000 augratin-23.5.16/augratin/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    25586 2023-05-16 19:37:32.000000 augratin-23.5.16/augratin/data/dialog.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22040 2023-02-17 19:16:23.000000 augratin-23.5.16/augratin/data/k6gte-augratin-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2015 2023-02-17 19:16:23.000000 augratin-23.5.16/augratin/data/k6gte-augratin-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6303 2023-02-17 19:16:23.000000 augratin-23.5.16/augratin/data/k6gte-augratin-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-17 19:16:23.000000 augratin-23.5.16/augratin/data/k6gte-augratin.desktop
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-16 19:45:37.193069 augratin-23.5.16/augratin/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.16/augratin/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13705 2023-05-16 19:37:32.000000 augratin-23.5.16/augratin/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2071 2023-03-28 14:10:04.000000 augratin-23.5.16/augratin/lib/omnirig_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-16 19:37:32.000000 augratin-23.5.16/augratin/lib/version.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-16 19:45:37.189069 augratin-23.5.16/augratin.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4644 2023-05-16 19:45:37.000000 augratin-23.5.16/augratin.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      591 2023-05-16 19:45:37.000000 augratin-23.5.16/augratin.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-16 19:45:37.000000 augratin-23.5.16/augratin.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-05-16 19:45:37.000000 augratin-23.5.16/augratin.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       71 2023-05-16 19:45:37.000000 augratin-23.5.16/augratin.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       31 2023-05-16 19:45:37.000000 augratin-23.5.16/augratin.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1142 2023-05-16 19:37:32.000000 augratin-23.5.16/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-16 19:45:37.194069 augratin-23.5.16/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-16 23:38:19.797559 augratin-23.5.16.1/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-02-19 00:59:20.000000 augratin-23.5.16.1/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4646 2023-05-16 23:38:19.797559 augratin-23.5.16.1/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3869 2023-05-16 19:43:59.000000 augratin-23.5.16.1/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-16 23:38:19.761558 augratin-23.5.16.1/augratin/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.16.1/augratin/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39599 2023-05-16 23:24:16.000000 augratin-23.5.16.1/augratin/__main__.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-16 23:38:19.795559 augratin-23.5.16.1/augratin/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-17 19:16:23.000000 augratin-23.5.16.1/augratin/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    25551 2023-05-16 23:31:35.000000 augratin-23.5.16.1/augratin/data/dialog.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22040 2023-02-17 19:16:23.000000 augratin-23.5.16.1/augratin/data/k6gte-augratin-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2015 2023-02-17 19:16:23.000000 augratin-23.5.16.1/augratin/data/k6gte-augratin-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6303 2023-02-17 19:16:23.000000 augratin-23.5.16.1/augratin/data/k6gte-augratin-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-17 19:16:23.000000 augratin-23.5.16.1/augratin/data/k6gte-augratin.desktop
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-16 23:38:19.796559 augratin-23.5.16.1/augratin/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.16.1/augratin/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13705 2023-05-16 19:37:32.000000 augratin-23.5.16.1/augratin/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2071 2023-03-28 14:10:04.000000 augratin-23.5.16.1/augratin/lib/omnirig_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       49 2023-05-16 23:33:39.000000 augratin-23.5.16.1/augratin/lib/version.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-16 23:38:19.786559 augratin-23.5.16.1/augratin.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4646 2023-05-16 23:38:19.000000 augratin-23.5.16.1/augratin.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      591 2023-05-16 23:38:19.000000 augratin-23.5.16.1/augratin.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-16 23:38:19.000000 augratin-23.5.16.1/augratin.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-05-16 23:38:19.000000 augratin-23.5.16.1/augratin.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       71 2023-05-16 23:38:19.000000 augratin-23.5.16.1/augratin.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       31 2023-05-16 23:38:19.000000 augratin-23.5.16.1/augratin.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1144 2023-05-16 23:33:41.000000 augratin-23.5.16.1/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-16 23:38:19.797559 augratin-23.5.16.1/setup.cfg
```

### Comparing `augratin-23.5.16/LICENSE` & `augratin-23.5.16.1/LICENSE`

 * *Files identical despite different names*

### Comparing `augratin-23.5.16/PKG-INFO` & `augratin-23.5.16.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augratin
-Version: 23.5.16
+Version: 23.5.16.1
 Summary: An aid for POTA hunters
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/augratin
 Project-URL: Bug Tracker, https://github.com/mbridak/augratin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `augratin-23.5.16/README.md` & `augratin-23.5.16.1/README.md`

 * *Files identical despite different names*

### Comparing `augratin-23.5.16/augratin/__main__.py` & `augratin-23.5.16.1/augratin/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,16 @@
 
     if sys.platform == "win32":
         from lib.omnirig_interface import OmniRigClient
 
 __author__ = "Michael C. Bridak, K6GTE"
 __license__ = "GNU General Public License v3.0"
 
+os.environ["QT_QPA_PLATFORMTHEME"] = "gnome"
+
 loader = pkgutil.get_loader("augratin")
 WORKING_PATH = os.path.dirname(loader.get_filename())
 
 logger = logging.getLogger("__name__")
 handler = logging.StreamHandler()
 formatter = logging.Formatter(
     datefmt="%H:%M:%S",
@@ -1048,15 +1050,15 @@
         "xdg-icon-resource install --size 32 --context apps --mode user "
         f"{WORKING_PATH}/data/k6gte-augratin-32.png k6gte-augratin"
     )
     os.system(f"xdg-desktop-menu install {WORKING_PATH}/data/k6gte-augratin.desktop")
 
 
 app = QtWidgets.QApplication(sys.argv)
-app.setStyle("Fusion")
+# app.setStyle("Fusion")
 font_dir = WORKING_PATH + "/data"
 families = load_fonts_from_dir(os.fspath(font_dir))
 logger.info(families)
 window = MainWindow()
 window.setWindowTitle(f"AuGratin v{__version__}")
 window.show()
 window.getspots()
```

### Comparing `augratin-23.5.16/augratin/data/JetBrainsMono-Regular.ttf` & `augratin-23.5.16.1/augratin/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `augratin-23.5.16/augratin/data/dialog.ui` & `augratin-23.5.16.1/augratin/data/dialog.ui`

 * *Files 1% similar despite different names*

#### Comparing `augratin-23.5.16/augratin/data/dialog.ui` & `augratin-23.5.16.1/augratin/data/dialog.ui`

```diff
@@ -21,19 +21,20 @@
         <family>JetBrains Mono</family>
         <pointsize>11</pointsize>
       </font>
     </property>
     <property name="windowTitle">
       <string>K6GTE AuGratin</string>
     </property>
-    <property name="styleSheet">
-      <string notr="true">background-color:rgb(45,45,45);
-color: rgb(211, 215, 207);</string>
-    </property>
     <widget class="QWidget" name="centralwidget">
+      <property name="font">
+        <font>
+          <family>JetBrains Mono</family>
+        </font>
+      </property>
       <layout class="QVBoxLayout" name="verticalLayout_3">
         <item>
           <layout class="QHBoxLayout" name="horizontalLayout" stretch="2,0,3">
             <property name="leftMargin">
               <number>9</number>
             </property>
             <property name="topMargin">
```

### Comparing `augratin-23.5.16/augratin/data/k6gte-augratin-128.png` & `augratin-23.5.16.1/augratin/data/k6gte-augratin-128.png`

 * *Files identical despite different names*

### Comparing `augratin-23.5.16/augratin/data/k6gte-augratin-32.png` & `augratin-23.5.16.1/augratin/data/k6gte-augratin-32.png`

 * *Files identical despite different names*

### Comparing `augratin-23.5.16/augratin/data/k6gte-augratin-64.png` & `augratin-23.5.16.1/augratin/data/k6gte-augratin-64.png`

 * *Files identical despite different names*

### Comparing `augratin-23.5.16/augratin/lib/cat_interface.py` & `augratin-23.5.16.1/augratin/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `augratin-23.5.16/augratin/lib/omnirig_interface.py` & `augratin-23.5.16.1/augratin/lib/omnirig_interface.py`

 * *Files identical despite different names*

### Comparing `augratin-23.5.16/augratin.egg-info/PKG-INFO` & `augratin-23.5.16.1/augratin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augratin
-Version: 23.5.16
+Version: 23.5.16.1
 Summary: An aid for POTA hunters
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/augratin
 Project-URL: Bug Tracker, https://github.com/mbridak/augratin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `augratin-23.5.16/augratin.egg-info/SOURCES.txt` & `augratin-23.5.16.1/augratin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `augratin-23.5.16/pyproject.toml` & `augratin-23.5.16.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "augratin" 
-version = "23.5.16"
+version = "23.5.16.1"
 description = "An aid for POTA hunters"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
```

