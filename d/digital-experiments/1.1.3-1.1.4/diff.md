# Comparing `tmp/digital-experiments-1.1.3.tar.gz` & `tmp/digital-experiments-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital-experiments-1.1.3.tar", last modified: Wed May 17 15:51:06 2023, max compression
+gzip compressed data, was "digital-experiments-1.1.4.tar", last modified: Wed May 17 16:02:17 2023, max compression
```

## Comparing `digital-experiments-1.1.3.tar` & `digital-experiments-1.1.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 15:51:06.194426 digital-experiments-1.1.3/
--rw-r--r--   0 john       (504) staff       (20)     1051 2022-11-18 07:34:19.000000 digital-experiments-1.1.3/LICENSE
--rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-17 15:51:06.194268 digital-experiments-1.1.3/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)     1008 2023-03-29 15:42:00.000000 digital-experiments-1.1.3/README.md
--rw-r--r--   0 john       (504) staff       (20)     1321 2023-05-17 15:50:59.000000 digital-experiments-1.1.3/pyproject.toml
--rw-r--r--   0 john       (504) staff       (20)       38 2023-05-17 15:51:06.194471 digital-experiments-1.1.3/setup.cfg
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 15:51:06.188239 digital-experiments-1.1.3/src/
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 15:51:06.190868 digital-experiments-1.1.3/src/digital_experiments/
--rw-r--r--   0 john       (504) staff       (20)      138 2023-05-17 15:50:59.000000 digital-experiments-1.1.3/src/digital_experiments/__init__.py
--rw-r--r--   0 john       (504) staff       (20)     6877 2023-05-17 15:48:49.000000 digital-experiments-1.1.3/src/digital_experiments/backends.py
--rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-17 15:42:42.000000 digital-experiments-1.1.3/src/digital_experiments/control_center.py
--rw-r--r--   0 john       (504) staff       (20)     4377 2023-05-17 15:50:20.000000 digital-experiments-1.1.3/src/digital_experiments/experiment.py
--rw-r--r--   0 john       (504) staff       (20)      402 2023-03-29 15:42:00.000000 digital-experiments-1.1.3/src/digital_experiments/inspection.py
--rw-r--r--   0 john       (504) staff       (20)     4450 2023-04-04 08:33:50.000000 digital-experiments-1.1.3/src/digital_experiments/minimize.py
--rw-r--r--   0 john       (504) staff       (20)      637 2023-03-29 15:42:00.000000 digital-experiments-1.1.3/src/digital_experiments/observation.py
--rw-r--r--   0 john       (504) staff       (20)      735 2023-05-10 08:20:22.000000 digital-experiments-1.1.3/src/digital_experiments/pretty.py
--rw-r--r--   0 john       (504) staff       (20)     2581 2023-05-09 14:17:13.000000 digital-experiments-1.1.3/src/digital_experiments/querying.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 15:51:06.191942 digital-experiments-1.1.3/src/digital_experiments/search/
--rw-r--r--   0 john       (504) staff       (20)     2897 2023-03-29 15:42:00.000000 digital-experiments-1.1.3/src/digital_experiments/search/skopt_suggest.py
--rw-r--r--   0 john       (504) staff       (20)     5381 2023-03-29 15:42:00.000000 digital-experiments-1.1.3/src/digital_experiments/search/space.py
--rw-r--r--   0 john       (504) staff       (20)     4218 2023-04-03 14:30:06.000000 digital-experiments-1.1.3/src/digital_experiments/search/suggest.py
--rw-r--r--   0 john       (504) staff       (20)     1682 2023-05-17 15:42:42.000000 digital-experiments-1.1.3/src/digital_experiments/timing.py
--rw-r--r--   0 john       (504) staff       (20)     5211 2023-05-17 15:42:42.000000 digital-experiments-1.1.3/src/digital_experiments/util.py
--rw-r--r--   0 john       (504) staff       (20)     3464 2023-03-29 15:42:00.000000 digital-experiments-1.1.3/src/digital_experiments/version_control.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 15:51:06.191577 digital-experiments-1.1.3/src/digital_experiments.egg-info/
--rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-17 15:51:06.000000 digital-experiments-1.1.3/src/digital_experiments.egg-info/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)     1147 2023-05-17 15:51:06.000000 digital-experiments-1.1.3/src/digital_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 john       (504) staff       (20)        1 2023-05-17 15:51:06.000000 digital-experiments-1.1.3/src/digital_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 john       (504) staff       (20)      160 2023-05-17 15:51:06.000000 digital-experiments-1.1.3/src/digital_experiments.egg-info/requires.txt
--rw-r--r--   0 john       (504) staff       (20)       20 2023-05-17 15:51:06.000000 digital-experiments-1.1.3/src/digital_experiments.egg-info/top_level.txt
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 15:51:06.193940 digital-experiments-1.1.3/tests/
--rw-r--r--   0 john       (504) staff       (20)     2083 2023-05-17 11:01:07.000000 digital-experiments-1.1.3/tests/test_backends.py
--rw-r--r--   0 john       (504) staff       (20)      844 2023-05-17 15:42:42.000000 digital-experiments-1.1.3/tests/test_control_center.py
--rw-r--r--   0 john       (504) staff       (20)     2099 2023-05-17 11:01:07.000000 digital-experiments-1.1.3/tests/test_experiment.py
--rw-r--r--   0 john       (504) staff       (20)      391 2023-05-17 11:01:07.000000 digital-experiments-1.1.3/tests/test_inspection.py
--rw-r--r--   0 john       (504) staff       (20)      632 2023-03-29 15:42:00.000000 digital-experiments-1.1.3/tests/test_minimize.py
--rw-r--r--   0 john       (504) staff       (20)      309 2023-05-17 11:01:07.000000 digital-experiments-1.1.3/tests/test_observation.py
--rw-r--r--   0 john       (504) staff       (20)      613 2023-05-10 08:20:22.000000 digital-experiments-1.1.3/tests/test_pretty.py
--rw-r--r--   0 john       (504) staff       (20)     1580 2023-05-09 14:17:13.000000 digital-experiments-1.1.3/tests/test_querying.py
--rw-r--r--   0 john       (504) staff       (20)     1596 2023-03-29 15:42:00.000000 digital-experiments-1.1.3/tests/test_space.py
--rw-r--r--   0 john       (504) staff       (20)     2188 2023-04-04 09:25:29.000000 digital-experiments-1.1.3/tests/test_suggest.py
--rw-r--r--   0 john       (504) staff       (20)      682 2023-05-17 15:42:42.000000 digital-experiments-1.1.3/tests/test_timing.py
--rw-r--r--   0 john       (504) staff       (20)     2820 2023-05-17 15:42:42.000000 digital-experiments-1.1.3/tests/test_util.py
--rw-r--r--   0 john       (504) staff       (20)     2397 2023-05-17 11:01:07.000000 digital-experiments-1.1.3/tests/test_version_control.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 16:02:17.805327 digital-experiments-1.1.4/
+-rw-r--r--   0 john       (504) staff       (20)     1051 2022-11-18 07:34:19.000000 digital-experiments-1.1.4/LICENSE
+-rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-17 16:02:17.805166 digital-experiments-1.1.4/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)     1008 2023-03-29 15:42:00.000000 digital-experiments-1.1.4/README.md
+-rw-r--r--   0 john       (504) staff       (20)     1321 2023-05-17 16:01:49.000000 digital-experiments-1.1.4/pyproject.toml
+-rw-r--r--   0 john       (504) staff       (20)       38 2023-05-17 16:02:17.805375 digital-experiments-1.1.4/setup.cfg
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 16:02:17.799152 digital-experiments-1.1.4/src/
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 16:02:17.801814 digital-experiments-1.1.4/src/digital_experiments/
+-rw-r--r--   0 john       (504) staff       (20)      138 2023-05-17 16:01:49.000000 digital-experiments-1.1.4/src/digital_experiments/__init__.py
+-rw-r--r--   0 john       (504) staff       (20)     6877 2023-05-17 15:48:49.000000 digital-experiments-1.1.4/src/digital_experiments/backends.py
+-rw-r--r--   0 john       (504) staff       (20)     2649 2023-05-17 16:01:39.000000 digital-experiments-1.1.4/src/digital_experiments/control_center.py
+-rw-r--r--   0 john       (504) staff       (20)     4377 2023-05-17 15:50:20.000000 digital-experiments-1.1.4/src/digital_experiments/experiment.py
+-rw-r--r--   0 john       (504) staff       (20)      402 2023-03-29 15:42:00.000000 digital-experiments-1.1.4/src/digital_experiments/inspection.py
+-rw-r--r--   0 john       (504) staff       (20)     4450 2023-04-04 08:33:50.000000 digital-experiments-1.1.4/src/digital_experiments/minimize.py
+-rw-r--r--   0 john       (504) staff       (20)      637 2023-03-29 15:42:00.000000 digital-experiments-1.1.4/src/digital_experiments/observation.py
+-rw-r--r--   0 john       (504) staff       (20)      735 2023-05-10 08:20:22.000000 digital-experiments-1.1.4/src/digital_experiments/pretty.py
+-rw-r--r--   0 john       (504) staff       (20)     2581 2023-05-09 14:17:13.000000 digital-experiments-1.1.4/src/digital_experiments/querying.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 16:02:17.803114 digital-experiments-1.1.4/src/digital_experiments/search/
+-rw-r--r--   0 john       (504) staff       (20)     2897 2023-03-29 15:42:00.000000 digital-experiments-1.1.4/src/digital_experiments/search/skopt_suggest.py
+-rw-r--r--   0 john       (504) staff       (20)     5381 2023-03-29 15:42:00.000000 digital-experiments-1.1.4/src/digital_experiments/search/space.py
+-rw-r--r--   0 john       (504) staff       (20)     4218 2023-04-03 14:30:06.000000 digital-experiments-1.1.4/src/digital_experiments/search/suggest.py
+-rw-r--r--   0 john       (504) staff       (20)     1682 2023-05-17 15:42:42.000000 digital-experiments-1.1.4/src/digital_experiments/timing.py
+-rw-r--r--   0 john       (504) staff       (20)     5211 2023-05-17 15:42:42.000000 digital-experiments-1.1.4/src/digital_experiments/util.py
+-rw-r--r--   0 john       (504) staff       (20)     3464 2023-03-29 15:42:00.000000 digital-experiments-1.1.4/src/digital_experiments/version_control.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 16:02:17.802676 digital-experiments-1.1.4/src/digital_experiments.egg-info/
+-rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-17 16:02:17.000000 digital-experiments-1.1.4/src/digital_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)     1147 2023-05-17 16:02:17.000000 digital-experiments-1.1.4/src/digital_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (504) staff       (20)        1 2023-05-17 16:02:17.000000 digital-experiments-1.1.4/src/digital_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (504) staff       (20)      160 2023-05-17 16:02:17.000000 digital-experiments-1.1.4/src/digital_experiments.egg-info/requires.txt
+-rw-r--r--   0 john       (504) staff       (20)       20 2023-05-17 16:02:17.000000 digital-experiments-1.1.4/src/digital_experiments.egg-info/top_level.txt
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 16:02:17.804949 digital-experiments-1.1.4/tests/
+-rw-r--r--   0 john       (504) staff       (20)     2083 2023-05-17 11:01:07.000000 digital-experiments-1.1.4/tests/test_backends.py
+-rw-r--r--   0 john       (504) staff       (20)      844 2023-05-17 15:42:42.000000 digital-experiments-1.1.4/tests/test_control_center.py
+-rw-r--r--   0 john       (504) staff       (20)     2099 2023-05-17 11:01:07.000000 digital-experiments-1.1.4/tests/test_experiment.py
+-rw-r--r--   0 john       (504) staff       (20)      391 2023-05-17 11:01:07.000000 digital-experiments-1.1.4/tests/test_inspection.py
+-rw-r--r--   0 john       (504) staff       (20)      632 2023-03-29 15:42:00.000000 digital-experiments-1.1.4/tests/test_minimize.py
+-rw-r--r--   0 john       (504) staff       (20)      309 2023-05-17 11:01:07.000000 digital-experiments-1.1.4/tests/test_observation.py
+-rw-r--r--   0 john       (504) staff       (20)      613 2023-05-10 08:20:22.000000 digital-experiments-1.1.4/tests/test_pretty.py
+-rw-r--r--   0 john       (504) staff       (20)     1580 2023-05-09 14:17:13.000000 digital-experiments-1.1.4/tests/test_querying.py
+-rw-r--r--   0 john       (504) staff       (20)     1596 2023-03-29 15:42:00.000000 digital-experiments-1.1.4/tests/test_space.py
+-rw-r--r--   0 john       (504) staff       (20)     2188 2023-04-04 09:25:29.000000 digital-experiments-1.1.4/tests/test_suggest.py
+-rw-r--r--   0 john       (504) staff       (20)      682 2023-05-17 15:42:42.000000 digital-experiments-1.1.4/tests/test_timing.py
+-rw-r--r--   0 john       (504) staff       (20)     2820 2023-05-17 15:42:42.000000 digital-experiments-1.1.4/tests/test_util.py
+-rw-r--r--   0 john       (504) staff       (20)     2397 2023-05-17 11:01:07.000000 digital-experiments-1.1.4/tests/test_version_control.py
```

### Comparing `digital-experiments-1.1.3/LICENSE` & `digital-experiments-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/PKG-INFO` & `digital-experiments-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-experiments
-Version: 1.1.3
+Version: 1.1.4
 Summary: Keep track of digital experiments.
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: Copyright 2022 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `digital-experiments-1.1.3/README.md` & `digital-experiments-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/pyproject.toml` & `digital-experiments-1.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digital-experiments"
-version = "1.1.3"
+version = "1.1.4"
 description = "Keep track of digital experiments."
 readme = "README.md"
 authors = [{ name = "John Gardner", email = "gardner.john97@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -41,15 +41,15 @@
     "pytest-cov",
 ]
 
 [project.urls]
 Homepage = "https://github.com/jla-gardner/digital-experiments"
 
 [tool.bumpver]
-current_version = "1.1.3"
+current_version = "1.1.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `digital-experiments-1.1.3/src/digital_experiments/backends.py` & `digital-experiments-1.1.4/src/digital_experiments/backends.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/src/digital_experiments/control_center.py` & `digital-experiments-1.1.4/src/digital_experiments/control_center.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     return __CURRENTLY_RUNNING[-1]
 
 
 def current_directory():
     """
     get the directory assigned to the currently running experiment
     """
-    current_run().directory
+    return current_run().directory
 
 
 @contextlib.contextmanager
 def additional_metadata(metadata: dict):
     """
     call outside of an experiment to register additional metadata
```

### Comparing `digital-experiments-1.1.3/src/digital_experiments/experiment.py` & `digital-experiments-1.1.4/src/digital_experiments/experiment.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/src/digital_experiments/minimize.py` & `digital-experiments-1.1.4/src/digital_experiments/minimize.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/src/digital_experiments/observation.py` & `digital-experiments-1.1.4/src/digital_experiments/observation.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/src/digital_experiments/pretty.py` & `digital-experiments-1.1.4/src/digital_experiments/pretty.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/src/digital_experiments/querying.py` & `digital-experiments-1.1.4/src/digital_experiments/querying.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/src/digital_experiments/search/skopt_suggest.py` & `digital-experiments-1.1.4/src/digital_experiments/search/skopt_suggest.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/src/digital_experiments/search/space.py` & `digital-experiments-1.1.4/src/digital_experiments/search/space.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/src/digital_experiments/search/suggest.py` & `digital-experiments-1.1.4/src/digital_experiments/search/suggest.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/src/digital_experiments/timing.py` & `digital-experiments-1.1.4/src/digital_experiments/timing.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/src/digital_experiments/util.py` & `digital-experiments-1.1.4/src/digital_experiments/util.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/src/digital_experiments/version_control.py` & `digital-experiments-1.1.4/src/digital_experiments/version_control.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/src/digital_experiments.egg-info/PKG-INFO` & `digital-experiments-1.1.4/src/digital_experiments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-experiments
-Version: 1.1.3
+Version: 1.1.4
 Summary: Keep track of digital experiments.
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: Copyright 2022 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `digital-experiments-1.1.3/src/digital_experiments.egg-info/SOURCES.txt` & `digital-experiments-1.1.4/src/digital_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/tests/test_backends.py` & `digital-experiments-1.1.4/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/tests/test_control_center.py` & `digital-experiments-1.1.4/tests/test_control_center.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/tests/test_experiment.py` & `digital-experiments-1.1.4/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/tests/test_minimize.py` & `digital-experiments-1.1.4/tests/test_minimize.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/tests/test_pretty.py` & `digital-experiments-1.1.4/tests/test_pretty.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/tests/test_querying.py` & `digital-experiments-1.1.4/tests/test_querying.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/tests/test_space.py` & `digital-experiments-1.1.4/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/tests/test_suggest.py` & `digital-experiments-1.1.4/tests/test_suggest.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/tests/test_timing.py` & `digital-experiments-1.1.4/tests/test_timing.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/tests/test_util.py` & `digital-experiments-1.1.4/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.3/tests/test_version_control.py` & `digital-experiments-1.1.4/tests/test_version_control.py`

 * *Files identical despite different names*

