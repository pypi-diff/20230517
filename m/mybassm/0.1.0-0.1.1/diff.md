# Comparing `tmp/mybassm-0.1.0.tar.gz` & `tmp/mybassm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mybassm-0.1.0.tar", last modified: Wed May 17 09:33:28 2023, max compression
+gzip compressed data, was "mybassm-0.1.1.tar", last modified: Wed May 17 10:36:56 2023, max compression
```

## Comparing `mybassm-0.1.0.tar` & `mybassm-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 anukzak    (501) staff       (20)        0 2023-05-17 09:33:28.154987 mybassm-0.1.0/
--rw-r--r--   0 anukzak    (501) staff       (20)      158 2023-05-17 07:55:21.000000 mybassm-0.1.0/AUTHORS.rst
--rw-r--r--   0 anukzak    (501) staff       (20)     3511 2023-05-17 07:55:21.000000 mybassm-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 anukzak    (501) staff       (20)       89 2023-05-17 07:55:21.000000 mybassm-0.1.0/HISTORY.rst
--rw-r--r--   0 anukzak    (501) staff       (20)     1074 2023-05-17 07:55:21.000000 mybassm-0.1.0/LICENSE
--rw-r--r--   0 anukzak    (501) staff       (20)      262 2023-05-17 07:55:21.000000 mybassm-0.1.0/MANIFEST.in
--rw-r--r--   0 anukzak    (501) staff       (20)      845 2023-05-17 09:33:28.155053 mybassm-0.1.0/PKG-INFO
--rw-r--r--   0 anukzak    (501) staff       (20)       57 2023-05-17 09:32:46.000000 mybassm-0.1.0/README.rst
-drwxr-xr-x   0 anukzak    (501) staff       (20)        0 2023-05-17 09:33:28.152907 mybassm-0.1.0/docs/
--rw-r--r--   0 anukzak    (501) staff       (20)      608 2023-05-17 07:55:21.000000 mybassm-0.1.0/docs/Makefile
--rw-r--r--   0 anukzak    (501) staff       (20)       28 2023-05-17 07:55:21.000000 mybassm-0.1.0/docs/authors.rst
--rwxr-xr-x   0 anukzak    (501) staff       (20)     4787 2023-05-17 07:55:21.000000 mybassm-0.1.0/docs/conf.py
--rw-r--r--   0 anukzak    (501) staff       (20)       33 2023-05-17 07:55:21.000000 mybassm-0.1.0/docs/contributing.rst
--rw-r--r--   0 anukzak    (501) staff       (20)       28 2023-05-17 07:55:21.000000 mybassm-0.1.0/docs/history.rst
--rw-r--r--   0 anukzak    (501) staff       (20)      304 2023-05-17 07:55:21.000000 mybassm-0.1.0/docs/index.rst
--rw-r--r--   0 anukzak    (501) staff       (20)     1118 2023-05-17 07:55:21.000000 mybassm-0.1.0/docs/installation.rst
--rw-r--r--   0 anukzak    (501) staff       (20)      769 2023-05-17 07:55:21.000000 mybassm-0.1.0/docs/make.bat
--rw-r--r--   0 anukzak    (501) staff       (20)       27 2023-05-17 07:55:21.000000 mybassm-0.1.0/docs/readme.rst
--rw-r--r--   0 anukzak    (501) staff       (20)       69 2023-05-17 07:55:21.000000 mybassm-0.1.0/docs/usage.rst
-drwxr-xr-x   0 anukzak    (501) staff       (20)        0 2023-05-17 09:33:28.153440 mybassm-0.1.0/mybassm/
--rw-r--r--   0 anukzak    (501) staff       (20)      204 2023-05-17 09:26:40.000000 mybassm-0.1.0/mybassm/__init__.py
--rw-r--r--   0 anukzak    (501) staff       (20)     5392 2023-05-17 08:16:31.000000 mybassm-0.1.0/mybassm/mybassm.py
-drwxr-xr-x   0 anukzak    (501) staff       (20)        0 2023-05-17 09:33:28.154420 mybassm-0.1.0/mybassm.egg-info/
--rw-r--r--   0 anukzak    (501) staff       (20)      845 2023-05-17 09:33:28.000000 mybassm-0.1.0/mybassm.egg-info/PKG-INFO
--rw-r--r--   0 anukzak    (501) staff       (20)      488 2023-05-17 09:33:28.000000 mybassm-0.1.0/mybassm.egg-info/SOURCES.txt
--rw-r--r--   0 anukzak    (501) staff       (20)        1 2023-05-17 09:33:28.000000 mybassm-0.1.0/mybassm.egg-info/dependency_links.txt
--rw-r--r--   0 anukzak    (501) staff       (20)        1 2023-05-17 08:23:13.000000 mybassm-0.1.0/mybassm.egg-info/not-zip-safe
--rw-r--r--   0 anukzak    (501) staff       (20)        8 2023-05-17 09:33:28.000000 mybassm-0.1.0/mybassm.egg-info/top_level.txt
--rw-r--r--   0 anukzak    (501) staff       (20)      424 2023-05-17 09:33:28.155363 mybassm-0.1.0/setup.cfg
--rw-r--r--   0 anukzak    (501) staff       (20)     1261 2023-05-17 07:55:21.000000 mybassm-0.1.0/setup.py
-drwxr-xr-x   0 anukzak    (501) staff       (20)        0 2023-05-17 09:33:28.154747 mybassm-0.1.0/tests/
--rw-r--r--   0 anukzak    (501) staff       (20)       37 2023-05-17 07:55:21.000000 mybassm-0.1.0/tests/__init__.py
--rw-r--r--   0 anukzak    (501) staff       (20)     1461 2023-05-17 08:02:51.000000 mybassm-0.1.0/tests/test_mybassm.py
+drwxr-xr-x   0 anukzak    (501) staff       (20)        0 2023-05-17 10:36:56.519829 mybassm-0.1.1/
+-rw-r--r--   0 anukzak    (501) staff       (20)      158 2023-05-17 07:55:21.000000 mybassm-0.1.1/AUTHORS.rst
+-rw-r--r--   0 anukzak    (501) staff       (20)     3511 2023-05-17 07:55:21.000000 mybassm-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 anukzak    (501) staff       (20)      128 2023-05-17 10:36:35.000000 mybassm-0.1.1/HISTORY.rst
+-rw-r--r--   0 anukzak    (501) staff       (20)     1074 2023-05-17 07:55:21.000000 mybassm-0.1.1/LICENSE
+-rw-r--r--   0 anukzak    (501) staff       (20)      262 2023-05-17 07:55:21.000000 mybassm-0.1.1/MANIFEST.in
+-rw-r--r--   0 anukzak    (501) staff       (20)     3385 2023-05-17 10:36:56.519916 mybassm-0.1.1/PKG-INFO
+-rw-r--r--   0 anukzak    (501) staff       (20)     2558 2023-05-17 10:24:51.000000 mybassm-0.1.1/README.rst
+drwxr-xr-x   0 anukzak    (501) staff       (20)        0 2023-05-17 10:36:56.517901 mybassm-0.1.1/docs/
+-rw-r--r--   0 anukzak    (501) staff       (20)      608 2023-05-17 07:55:21.000000 mybassm-0.1.1/docs/Makefile
+-rw-r--r--   0 anukzak    (501) staff       (20)       28 2023-05-17 07:55:21.000000 mybassm-0.1.1/docs/authors.rst
+-rwxr-xr-x   0 anukzak    (501) staff       (20)     4787 2023-05-17 07:55:21.000000 mybassm-0.1.1/docs/conf.py
+-rw-r--r--   0 anukzak    (501) staff       (20)       33 2023-05-17 07:55:21.000000 mybassm-0.1.1/docs/contributing.rst
+-rw-r--r--   0 anukzak    (501) staff       (20)       28 2023-05-17 07:55:21.000000 mybassm-0.1.1/docs/history.rst
+-rw-r--r--   0 anukzak    (501) staff       (20)      304 2023-05-17 07:55:21.000000 mybassm-0.1.1/docs/index.rst
+-rw-r--r--   0 anukzak    (501) staff       (20)     1118 2023-05-17 07:55:21.000000 mybassm-0.1.1/docs/installation.rst
+-rw-r--r--   0 anukzak    (501) staff       (20)      769 2023-05-17 07:55:21.000000 mybassm-0.1.1/docs/make.bat
+-rw-r--r--   0 anukzak    (501) staff       (20)       27 2023-05-17 07:55:21.000000 mybassm-0.1.1/docs/readme.rst
+-rw-r--r--   0 anukzak    (501) staff       (20)       69 2023-05-17 07:55:21.000000 mybassm-0.1.1/docs/usage.rst
+drwxr-xr-x   0 anukzak    (501) staff       (20)        0 2023-05-17 10:36:56.518226 mybassm-0.1.1/mybassm/
+-rw-r--r--   0 anukzak    (501) staff       (20)      204 2023-05-17 10:36:40.000000 mybassm-0.1.1/mybassm/__init__.py
+-rw-r--r--   0 anukzak    (501) staff       (20)     5392 2023-05-17 08:16:31.000000 mybassm-0.1.1/mybassm/mybassm.py
+drwxr-xr-x   0 anukzak    (501) staff       (20)        0 2023-05-17 10:36:56.519257 mybassm-0.1.1/mybassm.egg-info/
+-rw-r--r--   0 anukzak    (501) staff       (20)     3385 2023-05-17 10:36:56.000000 mybassm-0.1.1/mybassm.egg-info/PKG-INFO
+-rw-r--r--   0 anukzak    (501) staff       (20)      488 2023-05-17 10:36:56.000000 mybassm-0.1.1/mybassm.egg-info/SOURCES.txt
+-rw-r--r--   0 anukzak    (501) staff       (20)        1 2023-05-17 10:36:56.000000 mybassm-0.1.1/mybassm.egg-info/dependency_links.txt
+-rw-r--r--   0 anukzak    (501) staff       (20)        1 2023-05-17 08:23:13.000000 mybassm-0.1.1/mybassm.egg-info/not-zip-safe
+-rw-r--r--   0 anukzak    (501) staff       (20)        8 2023-05-17 10:36:56.000000 mybassm-0.1.1/mybassm.egg-info/top_level.txt
+-rw-r--r--   0 anukzak    (501) staff       (20)      424 2023-05-17 10:36:56.520244 mybassm-0.1.1/setup.cfg
+-rw-r--r--   0 anukzak    (501) staff       (20)     1261 2023-05-17 10:36:39.000000 mybassm-0.1.1/setup.py
+drwxr-xr-x   0 anukzak    (501) staff       (20)        0 2023-05-17 10:36:56.519585 mybassm-0.1.1/tests/
+-rw-r--r--   0 anukzak    (501) staff       (20)       37 2023-05-17 07:55:21.000000 mybassm-0.1.1/tests/__init__.py
+-rw-r--r--   0 anukzak    (501) staff       (20)     1461 2023-05-17 08:02:51.000000 mybassm-0.1.1/tests/test_mybassm.py
```

### Comparing `mybassm-0.1.0/CONTRIBUTING.rst` & `mybassm-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mybassm-0.1.0/LICENSE` & `mybassm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mybassm-0.1.0/docs/Makefile` & `mybassm-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mybassm-0.1.0/docs/conf.py` & `mybassm-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mybassm-0.1.0/docs/installation.rst` & `mybassm-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mybassm-0.1.0/docs/make.bat` & `mybassm-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mybassm-0.1.0/mybassm/mybassm.py` & `mybassm-0.1.1/mybassm/mybassm.py`

 * *Files identical despite different names*

### Comparing `mybassm-0.1.0/setup.py` & `mybassm-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords='mybassm',
     name='mybassm',
     packages=find_packages(include=['mybassm', 'mybassm.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/anukzak22/mybassm',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

### Comparing `mybassm-0.1.0/tests/test_mybassm.py` & `mybassm-0.1.1/tests/test_mybassm.py`

 * *Files identical despite different names*

