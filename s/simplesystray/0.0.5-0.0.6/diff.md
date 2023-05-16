# Comparing `tmp/simplesystray-0.0.5.tar.gz` & `tmp/simplesystray-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplesystray-0.0.5.tar", last modified: Tue May 16 22:03:04 2023, max compression
+gzip compressed data, was "simplesystray-0.0.6.tar", last modified: Tue May 16 22:14:08 2023, max compression
```

## Comparing `simplesystray-0.0.5.tar` & `simplesystray-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 22:03:04.953181 simplesystray-0.0.5/
--rw-rw-rw-   0        0        0     1499 2023-05-16 20:57:09.000000 simplesystray-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     5764 2023-05-16 22:03:04.952179 simplesystray-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5189 2023-05-16 21:39:36.000000 simplesystray-0.0.5/README.md
--rw-rw-rw-   0        0        0      653 2023-05-16 22:02:51.000000 simplesystray-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 22:03:04.953181 simplesystray-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 22:03:04.941178 simplesystray-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 22:03:04.945178 simplesystray-0.0.5/src/infi/
--rw-rw-rw-   0        0        0       57 2023-05-16 20:57:09.000000 simplesystray-0.0.5/src/infi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:03:04.947186 simplesystray-0.0.5/src/infi/systray/
--rw-rw-rw-   0        0        0       91 2023-05-16 20:57:09.000000 simplesystray-0.0.5/src/infi/systray/__init__.py
--rw-rw-rw-   0        0        0    12084 2023-05-16 21:40:55.000000 simplesystray-0.0.5/src/infi/systray/traybar.py
--rw-rw-rw-   0        0        0     6321 2023-05-16 20:57:09.000000 simplesystray-0.0.5/src/infi/systray/win32_adapter.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:03:04.951180 simplesystray-0.0.5/src/simplesystray.egg-info/
--rw-rw-rw-   0        0        0     5764 2023-05-16 22:03:04.000000 simplesystray-0.0.5/src/simplesystray.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-05-16 22:03:04.000000 simplesystray-0.0.5/src/simplesystray.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 22:03:04.000000 simplesystray-0.0.5/src/simplesystray.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-16 22:03:04.000000 simplesystray-0.0.5/src/simplesystray.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 22:03:04.951180 simplesystray-0.0.5/tests/
--rw-rw-rw-   0        0        0      756 2023-05-16 21:23:04.000000 simplesystray-0.0.5/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:14:08.706091 simplesystray-0.0.6/
+-rw-rw-rw-   0        0        0     1499 2023-05-16 20:57:09.000000 simplesystray-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     5764 2023-05-16 22:14:08.706091 simplesystray-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5189 2023-05-16 21:39:36.000000 simplesystray-0.0.6/README.md
+-rw-rw-rw-   0        0        0      653 2023-05-16 22:13:50.000000 simplesystray-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 22:14:08.706091 simplesystray-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 22:14:08.697091 simplesystray-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 22:14:08.701090 simplesystray-0.0.6/src/simplesystray/
+-rw-rw-rw-   0        0        0        0 2023-05-16 22:13:24.000000 simplesystray-0.0.6/src/simplesystray/__init__.py
+-rw-rw-rw-   0        0        0    12084 2023-05-16 21:40:55.000000 simplesystray-0.0.6/src/simplesystray/traybar.py
+-rw-rw-rw-   0        0        0     6321 2023-05-16 20:57:09.000000 simplesystray-0.0.6/src/simplesystray/win32_adapter.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:14:08.704093 simplesystray-0.0.6/src/simplesystray.egg-info/
+-rw-rw-rw-   0        0        0     5764 2023-05-16 22:14:08.000000 simplesystray-0.0.6/src/simplesystray.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-05-16 22:14:08.000000 simplesystray-0.0.6/src/simplesystray.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 22:14:08.000000 simplesystray-0.0.6/src/simplesystray.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-16 22:14:08.000000 simplesystray-0.0.6/src/simplesystray.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 22:14:08.705092 simplesystray-0.0.6/tests/
+-rw-rw-rw-   0        0        0      756 2023-05-16 21:23:04.000000 simplesystray-0.0.6/tests/test.py
```

### Comparing `simplesystray-0.0.5/LICENSE` & `simplesystray-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `simplesystray-0.0.5/PKG-INFO` & `simplesystray-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplesystray
-Version: 0.0.5
+Version: 0.0.6
 Summary: Adds support for a simple icon on the system tray, clone of infi-systray but maintained
 Author-email: actorpus <alex@actorpus.com>
 Project-URL: Homepage, https://github.com/actorpus/systrayv2
 Project-URL: Bug Tracker, https://github.com/actorpus/systrayv2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simplesystray-0.0.5/README.md` & `simplesystray-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `simplesystray-0.0.5/pyproject.toml` & `simplesystray-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "simplesystray"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="actorpus", email="alex@actorpus.com" },
 ]
 description = "Adds support for a simple icon on the system tray, clone of infi-systray but maintained"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simplesystray-0.0.5/src/infi/systray/traybar.py` & `simplesystray-0.0.6/src/simplesystray/traybar.py`

 * *Files identical despite different names*

### Comparing `simplesystray-0.0.5/src/infi/systray/win32_adapter.py` & `simplesystray-0.0.6/src/simplesystray/win32_adapter.py`

 * *Files identical despite different names*

### Comparing `simplesystray-0.0.5/src/simplesystray.egg-info/PKG-INFO` & `simplesystray-0.0.6/src/simplesystray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplesystray
-Version: 0.0.5
+Version: 0.0.6
 Summary: Adds support for a simple icon on the system tray, clone of infi-systray but maintained
 Author-email: actorpus <alex@actorpus.com>
 Project-URL: Homepage, https://github.com/actorpus/systrayv2
 Project-URL: Bug Tracker, https://github.com/actorpus/systrayv2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simplesystray-0.0.5/tests/test.py` & `simplesystray-0.0.6/tests/test.py`

 * *Files identical despite different names*

