# Comparing `tmp/deep_copilot-0.0.1.tar.gz` & `tmp/deep_copilot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_copilot-0.0.1.tar", last modified: Wed May 17 07:55:17 2023, max compression
+gzip compressed data, was "deep_copilot-0.0.2.tar", last modified: Wed May 17 08:11:32 2023, max compression
```

## Comparing `deep_copilot-0.0.1.tar` & `deep_copilot-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:55:17.931130 deep_copilot-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1940 2023-05-17 07:38:12.000000 deep_copilot-0.0.1/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    11558 2023-05-17 07:38:12.000000 deep_copilot-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      116 2023-05-17 07:38:12.000000 deep_copilot-0.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1809 2023-05-17 07:55:17.931130 deep_copilot-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1241 2023-05-17 07:38:12.000000 deep_copilot-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:55:17.930130 deep_copilot-0.0.1/deep_copilot/
--rw-r--r--   0 root         (0) root         (0)      130 2023-05-17 07:53:29.000000 deep_copilot-0.0.1/deep_copilot/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:55:17.931130 deep_copilot-0.0.1/deep_copilot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1809 2023-05-17 07:55:17.000000 deep_copilot-0.0.1/deep_copilot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      271 2023-05-17 07:55:17.000000 deep_copilot-0.0.1/deep_copilot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 07:55:17.000000 deep_copilot-0.0.1/deep_copilot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 07:55:17.000000 deep_copilot-0.0.1/deep_copilot.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 07:55:17.000000 deep_copilot-0.0.1/deep_copilot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1100 2023-05-17 07:41:17.000000 deep_copilot-0.0.1/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 07:55:17.931130 deep_copilot-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1968 2023-05-17 07:38:12.000000 deep_copilot-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:11:32.317305 deep_copilot-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-05-17 07:38:12.000000 deep_copilot-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    11558 2023-05-17 07:38:12.000000 deep_copilot-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      116 2023-05-17 07:38:12.000000 deep_copilot-0.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1809 2023-05-17 08:11:32.316305 deep_copilot-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-05-17 07:38:12.000000 deep_copilot-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:11:32.314305 deep_copilot-0.0.2/deep_copilot/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-05-17 07:53:29.000000 deep_copilot-0.0.2/deep_copilot/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:11:32.316305 deep_copilot-0.0.2/deep_copilot/mysql_tools/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-05-17 08:03:31.000000 deep_copilot-0.0.2/deep_copilot/mysql_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12399 2023-05-17 08:10:27.000000 deep_copilot-0.0.2/deep_copilot/mysql_tools/mysql_copilot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:11:32.316305 deep_copilot-0.0.2/deep_copilot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1809 2023-05-17 08:11:32.000000 deep_copilot-0.0.2/deep_copilot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      385 2023-05-17 08:11:32.000000 deep_copilot-0.0.2/deep_copilot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 08:11:32.000000 deep_copilot-0.0.2/deep_copilot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 07:55:17.000000 deep_copilot-0.0.2/deep_copilot.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-17 08:11:32.000000 deep_copilot-0.0.2/deep_copilot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 08:11:32.000000 deep_copilot-0.0.2/deep_copilot.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      511 2023-05-17 08:10:22.000000 deep_copilot-0.0.2/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 08:11:32.317305 deep_copilot-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1972 2023-05-17 08:11:27.000000 deep_copilot-0.0.2/setup.py
```

### Comparing `deep_copilot-0.0.1/CONTRIBUTING.md` & `deep_copilot-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.1/LICENSE` & `deep_copilot-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.1/PKG-INFO` & `deep_copilot-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: deep_copilot
-Version: 0.0.1
+Version: 0.0.2
 Summary: gyw toolkits
 Home-page: https://github.com/612twilight/deep_copilot/tree/master/
 Author: gyw
 Author-email: 240590367@qqq.com
 License: Apache Software License 2.0
 Keywords: anything not for deep learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pypi template
 
 > A minimal template for creating a pypi package
```

### Comparing `deep_copilot-0.0.1/README.md` & `deep_copilot-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.1/deep_copilot.egg-info/PKG-INFO` & `deep_copilot-0.0.2/deep_copilot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: deep-copilot
-Version: 0.0.1
+Version: 0.0.2
 Summary: gyw toolkits
 Home-page: https://github.com/612twilight/deep_copilot/tree/master/
 Author: gyw
 Author-email: 240590367@qqq.com
 License: Apache Software License 2.0
 Keywords: anything not for deep learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pypi template
 
 > A minimal template for creating a pypi package
```

### Comparing `deep_copilot-0.0.1/setup.py` & `deep_copilot-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 setup_cfg = {o:cfg[o] for o in cfg_keys}
 
 licenses = {
     'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
 }
 statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
     '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
-py_versions = '2.0 2.1 2.2 2.3 2.4 2.5 2.6 2.7 3.0 3.1 3.2 3.3 3.4 3.5 3.6 3.7 3.8'.split()
+py_versions = '2.0 2.1 2.2 2.3 2.4 2.5 2.6 2.7 3.0 3.1 3.2 3.3 3.4 3.5 3.6 3.7 3.8 3.9'.split()
 
 requirements = cfg.get('requirements','').split()
 lic = licenses[cfg['license']]
 min_python = cfg['min_python']
 
 setuptools.setup(
     name = cfg['lib_name'],
```

