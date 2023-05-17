# Comparing `tmp/pyquickconfig-0.1.tar.gz` & `tmp/pyquickconfig-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquickconfig-0.1.tar", last modified: Wed May 17 19:30:26 2023, max compression
+gzip compressed data, was "pyquickconfig-0.2.tar", last modified: Wed May 17 19:39:33 2023, max compression
```

## Comparing `pyquickconfig-0.1.tar` & `pyquickconfig-0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 austinibele   (501) staff       (20)        0 2023-05-17 19:30:26.923653 pyquickconfig-0.1/
--rw-r--r--   0 austinibele   (501) staff       (20)       40 2023-05-16 22:06:55.000000 pyquickconfig-0.1/.gitignore
--rw-r--r--   0 austinibele   (501) staff       (20)     1081 2023-05-17 19:23:49.000000 pyquickconfig-0.1/LICENSE
--rw-r--r--   0 austinibele   (501) staff       (20)      224 2023-05-17 19:30:26.923794 pyquickconfig-0.1/PKG-INFO
--rw-r--r--   0 austinibele   (501) staff       (20)     5357 2023-05-16 22:06:15.000000 pyquickconfig-0.1/README.md
-drwxr-xr-x   0 austinibele   (501) staff       (20)        0 2023-05-17 19:30:26.916991 pyquickconfig-0.1/example/
-drwxr-xr-x   0 austinibele   (501) staff       (20)        0 2023-05-17 19:30:26.919917 pyquickconfig-0.1/example/example_configs/
--rw-r--r--   0 austinibele   (501) staff       (20)      180 2023-05-16 22:06:15.000000 pyquickconfig-0.1/example/example_configs/filebased_config.json
--rw-r--r--   0 austinibele   (501) staff       (20)      184 2023-05-16 22:06:15.000000 pyquickconfig-0.1/example/example_configs/filebased_config_invalid.json
--rw-r--r--   0 austinibele   (501) staff       (20)       23 2023-05-16 22:06:15.000000 pyquickconfig-0.1/example/example_configs/model.json
--rw-r--r--   0 austinibele   (501) staff       (20)       27 2023-05-16 22:06:15.000000 pyquickconfig-0.1/example/example_configs/model_2.json
--rw-r--r--   0 austinibele   (501) staff       (20)      113 2023-05-16 22:06:15.000000 pyquickconfig-0.1/example/example_configs/subconfigs_defined_by_path.json
--rw-r--r--   0 austinibele   (501) staff       (20)       78 2023-05-16 22:06:15.000000 pyquickconfig-0.1/example/example_configs/training.json
--rw-r--r--   0 austinibele   (501) staff       (20)      337 2023-05-16 22:08:27.000000 pyquickconfig-0.1/example/main_config.py
--rw-r--r--   0 austinibele   (501) staff       (20)      361 2023-05-16 22:06:15.000000 pyquickconfig-0.1/example/model_config.py
--rw-r--r--   0 austinibele   (501) staff       (20)      757 2023-05-16 22:06:15.000000 pyquickconfig-0.1/example/training_config.py
-drwxr-xr-x   0 austinibele   (501) staff       (20)        0 2023-05-17 19:30:26.921285 pyquickconfig-0.1/quickconfig/
--rw-r--r--   0 austinibele   (501) staff       (20)     3526 2023-05-16 22:06:15.000000 pyquickconfig-0.1/quickconfig/base_config.py
--rw-r--r--   0 austinibele   (501) staff       (20)    16892 2023-05-16 22:06:15.000000 pyquickconfig-0.1/quickconfig/main_base.py
-drwxr-xr-x   0 austinibele   (501) staff       (20)        0 2023-05-17 19:30:26.922560 pyquickconfig-0.1/quickconfig/pyquickconfig.egg-info/
--rw-r--r--   0 austinibele   (501) staff       (20)      224 2023-05-17 19:30:26.000000 pyquickconfig-0.1/quickconfig/pyquickconfig.egg-info/PKG-INFO
--rw-r--r--   0 austinibele   (501) staff       (20)      696 2023-05-17 19:30:26.000000 pyquickconfig-0.1/quickconfig/pyquickconfig.egg-info/SOURCES.txt
--rw-r--r--   0 austinibele   (501) staff       (20)        1 2023-05-17 19:30:26.000000 pyquickconfig-0.1/quickconfig/pyquickconfig.egg-info/dependency_links.txt
--rw-r--r--   0 austinibele   (501) staff       (20)        1 2023-05-17 19:30:26.000000 pyquickconfig-0.1/quickconfig/pyquickconfig.egg-info/top_level.txt
--rw-r--r--   0 austinibele   (501) staff       (20)     2448 2023-05-16 22:06:15.000000 pyquickconfig-0.1/quickconfig/session_saver.py
--rw-r--r--   0 austinibele   (501) staff       (20)      103 2023-05-17 19:30:26.924322 pyquickconfig-0.1/setup.cfg
--rw-r--r--   0 austinibele   (501) staff       (20)      350 2023-05-17 19:30:24.000000 pyquickconfig-0.1/setup.py
-drwxr-xr-x   0 austinibele   (501) staff       (20)        0 2023-05-17 19:30:26.923061 pyquickconfig-0.1/tests/
--rw-r--r--   0 austinibele   (501) staff       (20)        0 2023-05-16 22:06:15.000000 pyquickconfig-0.1/tests/__init__.py
--rw-r--r--   0 austinibele   (501) staff       (20)     6653 2023-05-17 19:20:37.000000 pyquickconfig-0.1/tests/test.py
+drwxr-xr-x   0 austinibele   (501) staff       (20)        0 2023-05-17 19:39:33.564387 pyquickconfig-0.2/
+-rw-r--r--   0 austinibele   (501) staff       (20)       40 2023-05-16 22:06:55.000000 pyquickconfig-0.2/.gitignore
+-rw-r--r--   0 austinibele   (501) staff       (20)     1081 2023-05-17 19:23:49.000000 pyquickconfig-0.2/LICENSE
+-rw-r--r--   0 austinibele   (501) staff       (20)      224 2023-05-17 19:39:33.564535 pyquickconfig-0.2/PKG-INFO
+-rw-r--r--   0 austinibele   (501) staff       (20)     5357 2023-05-16 22:06:15.000000 pyquickconfig-0.2/README.md
+drwxr-xr-x   0 austinibele   (501) staff       (20)        0 2023-05-17 19:39:33.557669 pyquickconfig-0.2/example/
+drwxr-xr-x   0 austinibele   (501) staff       (20)        0 2023-05-17 19:39:33.561023 pyquickconfig-0.2/example/example_configs/
+-rw-r--r--   0 austinibele   (501) staff       (20)      180 2023-05-16 22:06:15.000000 pyquickconfig-0.2/example/example_configs/filebased_config.json
+-rw-r--r--   0 austinibele   (501) staff       (20)      184 2023-05-16 22:06:15.000000 pyquickconfig-0.2/example/example_configs/filebased_config_invalid.json
+-rw-r--r--   0 austinibele   (501) staff       (20)       23 2023-05-16 22:06:15.000000 pyquickconfig-0.2/example/example_configs/model.json
+-rw-r--r--   0 austinibele   (501) staff       (20)       27 2023-05-16 22:06:15.000000 pyquickconfig-0.2/example/example_configs/model_2.json
+-rw-r--r--   0 austinibele   (501) staff       (20)      113 2023-05-16 22:06:15.000000 pyquickconfig-0.2/example/example_configs/subconfigs_defined_by_path.json
+-rw-r--r--   0 austinibele   (501) staff       (20)       78 2023-05-16 22:06:15.000000 pyquickconfig-0.2/example/example_configs/training.json
+-rw-r--r--   0 austinibele   (501) staff       (20)      337 2023-05-16 22:08:27.000000 pyquickconfig-0.2/example/main_config.py
+-rw-r--r--   0 austinibele   (501) staff       (20)      361 2023-05-16 22:06:15.000000 pyquickconfig-0.2/example/model_config.py
+-rw-r--r--   0 austinibele   (501) staff       (20)      757 2023-05-16 22:06:15.000000 pyquickconfig-0.2/example/training_config.py
+drwxr-xr-x   0 austinibele   (501) staff       (20)        0 2023-05-17 19:39:33.562121 pyquickconfig-0.2/quickconfig/
+-rw-r--r--   0 austinibele   (501) staff       (20)     3526 2023-05-16 22:06:15.000000 pyquickconfig-0.2/quickconfig/base_config.py
+-rw-r--r--   0 austinibele   (501) staff       (20)    16892 2023-05-16 22:06:15.000000 pyquickconfig-0.2/quickconfig/main_base.py
+drwxr-xr-x   0 austinibele   (501) staff       (20)        0 2023-05-17 19:39:33.563284 pyquickconfig-0.2/quickconfig/pyquickconfig.egg-info/
+-rw-r--r--   0 austinibele   (501) staff       (20)      224 2023-05-17 19:39:33.000000 pyquickconfig-0.2/quickconfig/pyquickconfig.egg-info/PKG-INFO
+-rw-r--r--   0 austinibele   (501) staff       (20)      696 2023-05-17 19:39:33.000000 pyquickconfig-0.2/quickconfig/pyquickconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 austinibele   (501) staff       (20)        1 2023-05-17 19:39:33.000000 pyquickconfig-0.2/quickconfig/pyquickconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 austinibele   (501) staff       (20)        1 2023-05-17 19:39:33.000000 pyquickconfig-0.2/quickconfig/pyquickconfig.egg-info/top_level.txt
+-rw-r--r--   0 austinibele   (501) staff       (20)     2448 2023-05-16 22:06:15.000000 pyquickconfig-0.2/quickconfig/session_saver.py
+-rw-r--r--   0 austinibele   (501) staff       (20)      103 2023-05-17 19:39:33.565052 pyquickconfig-0.2/setup.cfg
+-rw-r--r--   0 austinibele   (501) staff       (20)      350 2023-05-17 19:39:23.000000 pyquickconfig-0.2/setup.py
+drwxr-xr-x   0 austinibele   (501) staff       (20)        0 2023-05-17 19:39:33.563820 pyquickconfig-0.2/tests/
+-rw-r--r--   0 austinibele   (501) staff       (20)        0 2023-05-16 22:06:15.000000 pyquickconfig-0.2/tests/__init__.py
+-rw-r--r--   0 austinibele   (501) staff       (20)     6653 2023-05-17 19:20:37.000000 pyquickconfig-0.2/tests/test.py
```

### Comparing `pyquickconfig-0.1/LICENSE` & `pyquickconfig-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyquickconfig-0.1/README.md` & `pyquickconfig-0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyquickconfig-0.1/example/training_config.py` & `pyquickconfig-0.2/example/training_config.py`

 * *Files identical despite different names*

### Comparing `pyquickconfig-0.1/quickconfig/base_config.py` & `pyquickconfig-0.2/quickconfig/base_config.py`

 * *Files identical despite different names*

### Comparing `pyquickconfig-0.1/quickconfig/main_base.py` & `pyquickconfig-0.2/quickconfig/main_base.py`

 * *Files identical despite different names*

### Comparing `pyquickconfig-0.1/quickconfig/pyquickconfig.egg-info/SOURCES.txt` & `pyquickconfig-0.2/quickconfig/pyquickconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyquickconfig-0.1/quickconfig/session_saver.py` & `pyquickconfig-0.2/quickconfig/session_saver.py`

 * *Files identical despite different names*

### Comparing `pyquickconfig-0.1/tests/test.py` & `pyquickconfig-0.2/tests/test.py`

 * *Files identical despite different names*

