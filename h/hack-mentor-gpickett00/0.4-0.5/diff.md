# Comparing `tmp/hack_mentor_gpickett00-0.4.tar.gz` & `tmp/hack_mentor_gpickett00-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hack_mentor_gpickett00-0.4.tar", last modified: Tue May 16 22:21:39 2023, max compression
+gzip compressed data, was "hack_mentor_gpickett00-0.5.tar", last modified: Tue May 16 22:23:21 2023, max compression
```

## Comparing `hack_mentor_gpickett00-0.4.tar` & `hack_mentor_gpickett00-0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 georgepickett   (502) staff       (20)        0 2023-05-16 22:21:39.194686 hack_mentor_gpickett00-0.4/
--rw-r--r--   0 georgepickett   (502) staff       (20)     2495 2023-05-16 22:21:39.194156 hack_mentor_gpickett00-0.4/PKG-INFO
--rw-r--r--   0 georgepickett   (502) staff       (20)     1969 2023-05-16 22:19:14.000000 hack_mentor_gpickett00-0.4/README.md
-drwxr-xr-x   0 georgepickett   (502) staff       (20)        0 2023-05-16 22:21:39.189626 hack_mentor_gpickett00-0.4/hack_mentor/
--rw-r--r--   0 georgepickett   (502) staff       (20)        0 2023-05-16 19:34:27.000000 hack_mentor_gpickett00-0.4/hack_mentor/__init__.py
--rw-r--r--   0 georgepickett   (502) staff       (20)     2382 2023-05-16 21:39:13.000000 hack_mentor_gpickett00-0.4/hack_mentor/main.py
--rw-r--r--   0 georgepickett   (502) staff       (20)     1570 2023-05-16 21:29:27.000000 hack_mentor_gpickett00-0.4/hack_mentor/prompts.py
-drwxr-xr-x   0 georgepickett   (502) staff       (20)        0 2023-05-16 22:21:39.193263 hack_mentor_gpickett00-0.4/hack_mentor_gpickett00.egg-info/
--rw-r--r--   0 georgepickett   (502) staff       (20)     2495 2023-05-16 22:21:39.000000 hack_mentor_gpickett00-0.4/hack_mentor_gpickett00.egg-info/PKG-INFO
--rw-r--r--   0 georgepickett   (502) staff       (20)      333 2023-05-16 22:21:39.000000 hack_mentor_gpickett00-0.4/hack_mentor_gpickett00.egg-info/SOURCES.txt
--rw-r--r--   0 georgepickett   (502) staff       (20)        1 2023-05-16 22:21:39.000000 hack_mentor_gpickett00-0.4/hack_mentor_gpickett00.egg-info/dependency_links.txt
--rw-r--r--   0 georgepickett   (502) staff       (20)       54 2023-05-16 22:21:39.000000 hack_mentor_gpickett00-0.4/hack_mentor_gpickett00.egg-info/entry_points.txt
--rw-r--r--   0 georgepickett   (502) staff       (20)       12 2023-05-16 22:21:39.000000 hack_mentor_gpickett00-0.4/hack_mentor_gpickett00.egg-info/top_level.txt
--rw-r--r--   0 georgepickett   (502) staff       (20)      533 2023-05-16 22:21:01.000000 hack_mentor_gpickett00-0.4/pyproject.toml
--rw-r--r--   0 georgepickett   (502) staff       (20)       38 2023-05-16 22:21:39.194845 hack_mentor_gpickett00-0.4/setup.cfg
--rw-r--r--   0 georgepickett   (502) staff       (20)      245 2023-05-16 22:20:46.000000 hack_mentor_gpickett00-0.4/setup.py
+drwxr-xr-x   0 georgepickett   (502) staff       (20)        0 2023-05-16 22:23:21.781701 hack_mentor_gpickett00-0.5/
+-rw-r--r--   0 georgepickett   (502) staff       (20)     2495 2023-05-16 22:23:21.781114 hack_mentor_gpickett00-0.5/PKG-INFO
+-rw-r--r--   0 georgepickett   (502) staff       (20)     1969 2023-05-16 22:19:14.000000 hack_mentor_gpickett00-0.5/README.md
+drwxr-xr-x   0 georgepickett   (502) staff       (20)        0 2023-05-16 22:23:21.776676 hack_mentor_gpickett00-0.5/hack_mentor/
+-rw-r--r--   0 georgepickett   (502) staff       (20)        0 2023-05-16 19:34:27.000000 hack_mentor_gpickett00-0.5/hack_mentor/__init__.py
+-rw-r--r--   0 georgepickett   (502) staff       (20)     2382 2023-05-16 21:39:13.000000 hack_mentor_gpickett00-0.5/hack_mentor/main.py
+-rw-r--r--   0 georgepickett   (502) staff       (20)     1570 2023-05-16 21:29:27.000000 hack_mentor_gpickett00-0.5/hack_mentor/prompts.py
+drwxr-xr-x   0 georgepickett   (502) staff       (20)        0 2023-05-16 22:23:21.780064 hack_mentor_gpickett00-0.5/hack_mentor_gpickett00.egg-info/
+-rw-r--r--   0 georgepickett   (502) staff       (20)     2495 2023-05-16 22:23:21.000000 hack_mentor_gpickett00-0.5/hack_mentor_gpickett00.egg-info/PKG-INFO
+-rw-r--r--   0 georgepickett   (502) staff       (20)      378 2023-05-16 22:23:21.000000 hack_mentor_gpickett00-0.5/hack_mentor_gpickett00.egg-info/SOURCES.txt
+-rw-r--r--   0 georgepickett   (502) staff       (20)        1 2023-05-16 22:23:21.000000 hack_mentor_gpickett00-0.5/hack_mentor_gpickett00.egg-info/dependency_links.txt
+-rw-r--r--   0 georgepickett   (502) staff       (20)       54 2023-05-16 22:23:21.000000 hack_mentor_gpickett00-0.5/hack_mentor_gpickett00.egg-info/entry_points.txt
+-rw-r--r--   0 georgepickett   (502) staff       (20)       42 2023-05-16 22:23:21.000000 hack_mentor_gpickett00-0.5/hack_mentor_gpickett00.egg-info/requires.txt
+-rw-r--r--   0 georgepickett   (502) staff       (20)       12 2023-05-16 22:23:21.000000 hack_mentor_gpickett00-0.5/hack_mentor_gpickett00.egg-info/top_level.txt
+-rw-r--r--   0 georgepickett   (502) staff       (20)      533 2023-05-16 22:23:08.000000 hack_mentor_gpickett00-0.5/pyproject.toml
+-rw-r--r--   0 georgepickett   (502) staff       (20)       38 2023-05-16 22:23:21.781866 hack_mentor_gpickett00-0.5/setup.cfg
+-rw-r--r--   0 georgepickett   (502) staff       (20)      371 2023-05-16 22:22:59.000000 hack_mentor_gpickett00-0.5/setup.py
```

### Comparing `hack_mentor_gpickett00-0.4/PKG-INFO` & `hack_mentor_gpickett00-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hack_mentor_gpickett00
-Version: 0.4
+Version: 0.5
 Summary: GPT4 in your terminal, watching you code and giving feedback
 Author-email: George Pickett <gpickett00@gmail.com>
 Project-URL: Homepage, https://github.com/grp06/hack_mentor
 Project-URL: Bug Tracker, https://github.com/grp06/hack_mentor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hack_mentor_gpickett00-0.4/README.md` & `hack_mentor_gpickett00-0.5/README.md`

 * *Files identical despite different names*

### Comparing `hack_mentor_gpickett00-0.4/hack_mentor/main.py` & `hack_mentor_gpickett00-0.5/hack_mentor/main.py`

 * *Files identical despite different names*

### Comparing `hack_mentor_gpickett00-0.4/hack_mentor/prompts.py` & `hack_mentor_gpickett00-0.5/hack_mentor/prompts.py`

 * *Files identical despite different names*

### Comparing `hack_mentor_gpickett00-0.4/hack_mentor_gpickett00.egg-info/PKG-INFO` & `hack_mentor_gpickett00-0.5/hack_mentor_gpickett00.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hack-mentor-gpickett00
-Version: 0.4
+Version: 0.5
 Summary: GPT4 in your terminal, watching you code and giving feedback
 Author-email: George Pickett <gpickett00@gmail.com>
 Project-URL: Homepage, https://github.com/grp06/hack_mentor
 Project-URL: Bug Tracker, https://github.com/grp06/hack_mentor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hack_mentor_gpickett00-0.4/pyproject.toml` & `hack_mentor_gpickett00-0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hack_mentor_gpickett00"
-version = "0.4"
+version = "0.5"
 authors = [
   { name="George Pickett", email="gpickett00@gmail.com" },
 ]
 description = "GPT4 in your terminal, watching you code and giving feedback"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

