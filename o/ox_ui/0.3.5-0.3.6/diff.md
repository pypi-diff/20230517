# Comparing `tmp/ox_ui-0.3.5.tar.gz` & `tmp/ox_ui-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ox_ui-0.3.5.tar", last modified: Mon May 15 19:12:33 2023, max compression
+gzip compressed data, was "ox_ui-0.3.6.tar", last modified: Wed May 17 19:40:12 2023, max compression
```

## Comparing `ox_ui-0.3.5.tar` & `ox_ui-0.3.6.tar`

### file list

```diff
@@ -1,40 +1,46 @@
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 19:12:33.767293 ox_ui-0.3.5/
--rw-------   0 emin      (1000) emin      (1000)     1129 2019-07-23 18:08:30.000000 ox_ui-0.3.5/.gitignore
--rw-------   0 emin      (1000) emin      (1000)     1325 2019-07-23 18:03:49.000000 ox_ui-0.3.5/LICENSE.txt
--rw-------   0 emin      (1000) emin      (1000)       56 2019-07-24 15:29:34.000000 ox_ui-0.3.5/MANIFEST.in
--rw-rw-r--   0 emin      (1000) emin      (1000)      535 2023-05-15 19:12:33.767293 ox_ui-0.3.5/PKG-INFO
--rw-------   0 emin      (1000) emin      (1000)       82 2019-07-23 18:08:09.000000 ox_ui-0.3.5/README.org
--rw-rw-r--   0 emin      (1000) emin      (1000)       93 2022-04-19 15:06:12.000000 ox_ui-0.3.5/README.rst
--rw-------   0 emin      (1000) emin      (1000)       73 2019-07-23 18:03:49.000000 ox_ui-0.3.5/conftest.py
--rw-------   0 emin      (1000) emin      (1000)      459 2019-07-23 18:04:11.000000 ox_ui-0.3.5/makefile
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 19:12:33.763293 ox_ui-0.3.5/ox_ui/
--rw-rw-r--   0 emin      (1000) emin      (1000)       67 2023-05-15 19:11:41.000000 ox_ui-0.3.5/ox_ui/__init__.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 19:12:33.767293 ox_ui-0.3.5/ox_ui/assets/
--rw-------   0 emin      (1000) emin      (1000)       55 2019-07-23 18:01:55.000000 ox_ui-0.3.5/ox_ui/assets/__init__.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 19:12:33.767293 ox_ui-0.3.5/ox_ui/assets/css/
--rw-------   0 emin      (1000) emin      (1000)       19 2019-07-23 18:01:55.000000 ox_ui-0.3.5/ox_ui/assets/css/__init__.py
--rw-------   0 emin      (1000) emin      (1000)    23563 2019-07-23 18:01:55.000000 ox_ui-0.3.5/ox_ui/assets/css/w3.css
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 19:12:33.767293 ox_ui-0.3.5/ox_ui/core/
--rw-------   0 emin      (1000) emin      (1000)       31 2019-07-23 18:01:55.000000 ox_ui-0.3.5/ox_ui/core/__init__.py
--rw-rw-r--   0 emin      (1000) emin      (1000)    13909 2023-05-15 18:12:01.000000 ox_ui-0.3.5/ox_ui/core/c2f.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     7069 2022-05-09 17:50:36.000000 ox_ui-0.3.5/ox_ui/core/c2g.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     5914 2023-05-15 19:11:41.000000 ox_ui-0.3.5/ox_ui/core/decorators.py
--rw-------   0 emin      (1000) emin      (1000)     1405 2019-07-23 18:01:55.000000 ox_ui-0.3.5/ox_ui/core/sample_wtf.html
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 19:12:33.767293 ox_ui-0.3.5/ox_ui/test_tools/
--rw-------   0 emin      (1000) emin      (1000)       39 2019-07-23 18:01:55.000000 ox_ui-0.3.5/ox_ui/test_tools/__init__.py
--rw-------   0 emin      (1000) emin      (1000)     2938 2019-07-23 18:01:55.000000 ox_ui-0.3.5/ox_ui/test_tools/server_tools.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 19:12:33.763293 ox_ui-0.3.5/ox_ui.egg-info/
--rw-------   0 emin      (1000) emin      (1000)      535 2023-05-15 19:12:33.000000 ox_ui-0.3.5/ox_ui.egg-info/PKG-INFO
--rw-------   0 emin      (1000) emin      (1000)      629 2023-05-15 19:12:33.000000 ox_ui-0.3.5/ox_ui.egg-info/SOURCES.txt
--rw-------   0 emin      (1000) emin      (1000)        1 2023-05-15 19:12:33.000000 ox_ui-0.3.5/ox_ui.egg-info/dependency_links.txt
--rw-------   0 emin      (1000) emin      (1000)       40 2023-05-15 19:12:33.000000 ox_ui-0.3.5/ox_ui.egg-info/entry_points.txt
--rw-------   0 emin      (1000) emin      (1000)        7 2023-05-15 19:12:33.000000 ox_ui-0.3.5/ox_ui.egg-info/requires.txt
--rw-------   0 emin      (1000) emin      (1000)        6 2023-05-15 19:12:33.000000 ox_ui-0.3.5/ox_ui.egg-info/top_level.txt
--rw-rw-r--   0 emin      (1000) emin      (1000)      689 2023-05-15 18:12:44.000000 ox_ui-0.3.5/requirements.txt
--rw-rw-r--   0 emin      (1000) emin      (1000)       38 2023-05-15 19:12:33.767293 ox_ui-0.3.5/setup.cfg
--rw-------   0 emin      (1000) emin      (1000)     1941 2019-07-23 18:05:48.000000 ox_ui-0.3.5/setup.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 19:12:33.763293 ox_ui-0.3.5/tests/
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-15 19:12:33.767293 ox_ui-0.3.5/tests/flask/
--rw-rw-r--   0 emin      (1000) emin      (1000)     2538 2023-05-15 19:11:41.000000 ox_ui-0.3.5/tests/flask/c2f_app.py
--rw-------   0 emin      (1000) emin      (1000)      219 2019-07-23 18:01:55.000000 ox_ui-0.3.5/tests/flask/minimal_app.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     3655 2023-05-15 18:12:01.000000 ox_ui-0.3.5/tests/flask/test_simple_c2f.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-17 19:40:12.049552 ox_ui-0.3.6/
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-17 19:40:12.045552 ox_ui-0.3.6/.github/
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-17 19:40:12.049552 ox_ui-0.3.6/.github/workflows/
+-rw-rw-r--   0 emin      (1000) emin      (1000)      337 2022-04-19 15:06:12.000000 ox_ui-0.3.6/.github/workflows/makefile.yml
+-rw-------   0 emin      (1000) emin      (1000)     1129 2019-07-23 18:08:30.000000 ox_ui-0.3.6/.gitignore
+-rw-------   0 emin      (1000) emin      (1000)     1325 2019-07-23 18:03:49.000000 ox_ui-0.3.6/LICENSE.txt
+-rw-------   0 emin      (1000) emin      (1000)       56 2019-07-24 15:29:34.000000 ox_ui-0.3.6/MANIFEST.in
+-rw-rw-r--   0 emin      (1000) emin      (1000)     3131 2023-05-17 19:40:12.049552 ox_ui-0.3.6/PKG-INFO
+-rw-rw-r--   0 emin      (1000) emin      (1000)     2131 2023-05-17 19:39:32.000000 ox_ui-0.3.6/README.org
+-rw-rw-r--   0 emin      (1000) emin      (1000)     2185 2023-05-17 19:40:11.000000 ox_ui-0.3.6/README.rst
+-rw-------   0 emin      (1000) emin      (1000)       73 2019-07-23 18:03:49.000000 ox_ui-0.3.6/conftest.py
+-rw-------   0 emin      (1000) emin      (1000)      459 2019-07-23 18:04:11.000000 ox_ui-0.3.6/makefile
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-17 19:40:12.049552 ox_ui-0.3.6/ox_ui/
+-rw-rw-r--   0 emin      (1000) emin      (1000)       67 2023-05-17 19:39:32.000000 ox_ui-0.3.6/ox_ui/__init__.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-17 19:40:12.049552 ox_ui-0.3.6/ox_ui/assets/
+-rw-------   0 emin      (1000) emin      (1000)       55 2019-07-23 18:01:55.000000 ox_ui-0.3.6/ox_ui/assets/__init__.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-17 19:40:12.049552 ox_ui-0.3.6/ox_ui/assets/css/
+-rw-------   0 emin      (1000) emin      (1000)       19 2019-07-23 18:01:55.000000 ox_ui-0.3.6/ox_ui/assets/css/__init__.py
+-rw-------   0 emin      (1000) emin      (1000)    23563 2019-07-23 18:01:55.000000 ox_ui-0.3.6/ox_ui/assets/css/w3.css
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-17 19:40:12.049552 ox_ui-0.3.6/ox_ui/core/
+-rw-------   0 emin      (1000) emin      (1000)       31 2019-07-23 18:01:55.000000 ox_ui-0.3.6/ox_ui/core/__init__.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)    13909 2023-05-15 18:12:01.000000 ox_ui-0.3.6/ox_ui/core/c2f.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     7069 2022-05-09 17:50:36.000000 ox_ui-0.3.6/ox_ui/core/c2g.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     8746 2023-05-17 19:39:32.000000 ox_ui-0.3.6/ox_ui/core/decorators.py
+-rw-------   0 emin      (1000) emin      (1000)     1405 2019-07-23 18:01:55.000000 ox_ui-0.3.6/ox_ui/core/sample_wtf.html
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-17 19:40:12.049552 ox_ui-0.3.6/ox_ui/test_tools/
+-rw-------   0 emin      (1000) emin      (1000)       39 2019-07-23 18:01:55.000000 ox_ui-0.3.6/ox_ui/test_tools/__init__.py
+-rw-------   0 emin      (1000) emin      (1000)     2938 2019-07-23 18:01:55.000000 ox_ui-0.3.6/ox_ui/test_tools/server_tools.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-17 19:40:12.049552 ox_ui-0.3.6/ox_ui.egg-info/
+-rw-------   0 emin      (1000) emin      (1000)     3131 2023-05-17 19:40:11.000000 ox_ui-0.3.6/ox_ui.egg-info/PKG-INFO
+-rw-------   0 emin      (1000) emin      (1000)      709 2023-05-17 19:40:12.000000 ox_ui-0.3.6/ox_ui.egg-info/SOURCES.txt
+-rw-------   0 emin      (1000) emin      (1000)        1 2023-05-17 19:40:11.000000 ox_ui-0.3.6/ox_ui.egg-info/dependency_links.txt
+-rw-------   0 emin      (1000) emin      (1000)       40 2023-05-17 19:40:11.000000 ox_ui-0.3.6/ox_ui.egg-info/entry_points.txt
+-rw-------   0 emin      (1000) emin      (1000)        7 2023-05-17 19:40:11.000000 ox_ui-0.3.6/ox_ui.egg-info/requires.txt
+-rw-------   0 emin      (1000) emin      (1000)        6 2023-05-17 19:40:11.000000 ox_ui-0.3.6/ox_ui.egg-info/top_level.txt
+-rw-rw-r--   0 emin      (1000) emin      (1000)      689 2023-05-17 19:39:39.000000 ox_ui-0.3.6/requirements.txt
+-rw-rw-r--   0 emin      (1000) emin      (1000)       38 2023-05-17 19:40:12.049552 ox_ui-0.3.6/setup.cfg
+-rw-------   0 emin      (1000) emin      (1000)     1941 2019-07-23 18:05:48.000000 ox_ui-0.3.6/setup.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-17 19:40:12.045552 ox_ui-0.3.6/tests/
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-17 19:40:12.049552 ox_ui-0.3.6/tests/flask/
+-rw-rw-r--   0 emin      (1000) emin      (1000)     2538 2023-05-17 19:38:21.000000 ox_ui-0.3.6/tests/flask/c2f_app.py
+-rw-------   0 emin      (1000) emin      (1000)      219 2019-07-23 18:01:55.000000 ox_ui-0.3.6/tests/flask/minimal_app.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     3655 2023-05-15 18:12:01.000000 ox_ui-0.3.6/tests/flask/test_simple_c2f.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-05-17 19:40:12.049552 ox_ui-0.3.6/tests/text/
+-rw-rw-r--   0 emin      (1000) emin      (1000)       42 2022-04-19 15:06:12.000000 ox_ui-0.3.6/tests/text/__init__.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     2139 2023-05-15 17:41:26.000000 ox_ui-0.3.6/tests/text/test_basics.py
```

### Comparing `ox_ui-0.3.5/.gitignore` & `ox_ui-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.5/LICENSE.txt` & `ox_ui-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.5/ox_ui/assets/css/w3.css` & `ox_ui-0.3.6/ox_ui/assets/css/w3.css`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.5/ox_ui/core/c2f.py` & `ox_ui-0.3.6/ox_ui/core/c2f.py`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.5/ox_ui/core/c2g.py` & `ox_ui-0.3.6/ox_ui/core/c2g.py`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.5/ox_ui/core/sample_wtf.html` & `ox_ui-0.3.6/ox_ui/core/sample_wtf.html`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.5/ox_ui/test_tools/server_tools.py` & `ox_ui-0.3.6/ox_ui/test_tools/server_tools.py`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.5/ox_ui.egg-info/SOURCES.txt` & `ox_ui-0.3.6/ox_ui.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 MANIFEST.in
 README.org
 README.rst
 conftest.py
 makefile
 requirements.txt
 setup.py
+.github/workflows/makefile.yml
 ox_ui/__init__.py
 ox_ui.egg-info/PKG-INFO
 ox_ui.egg-info/SOURCES.txt
 ox_ui.egg-info/dependency_links.txt
 ox_ui.egg-info/entry_points.txt
 ox_ui.egg-info/requires.txt
 ox_ui.egg-info/top_level.txt
@@ -22,8 +23,10 @@
 ox_ui/core/c2g.py
 ox_ui/core/decorators.py
 ox_ui/core/sample_wtf.html
 ox_ui/test_tools/__init__.py
 ox_ui/test_tools/server_tools.py
 tests/flask/c2f_app.py
 tests/flask/minimal_app.py
-tests/flask/test_simple_c2f.py
+tests/flask/test_simple_c2f.py
+tests/text/__init__.py
+tests/text/test_basics.py
```

### Comparing `ox_ui-0.3.5/requirements.txt` & `ox_ui-0.3.6/requirements.txt`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 certifi==2022.12.7
 charset-normalizer==2.0.12
 click==8.0.4
 dill==0.3.4
 execnet==1.9.0
 eyap==0.9.3
 flake8==4.0.1
-Flask==2.0.3
+Flask==2.2.5
 Flask-WTF==1.0.0
 idna==3.3
 iniconfig==1.1.1
 isort==5.10.1
 itsdangerous==2.1.2
 Jinja2==3.1.0
 lazy-object-proxy==1.7.1
```

### Comparing `ox_ui-0.3.5/setup.py` & `ox_ui-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.5/tests/flask/c2f_app.py` & `ox_ui-0.3.6/tests/flask/c2f_app.py`

 * *Files identical despite different names*

### Comparing `ox_ui-0.3.5/tests/flask/test_simple_c2f.py` & `ox_ui-0.3.6/tests/flask/test_simple_c2f.py`

 * *Files identical despite different names*

