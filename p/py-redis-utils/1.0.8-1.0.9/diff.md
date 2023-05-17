# Comparing `tmp/py-redis-utils-1.0.8.tar.gz` & `tmp/py-redis-utils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-redis-utils-1.0.8.tar", last modified: Fri Apr 14 11:38:37 2023, max compression
+gzip compressed data, was "py-redis-utils-1.0.9.tar", last modified: Wed May 17 08:56:44 2023, max compression
```

## Comparing `py-redis-utils-1.0.8.tar` & `py-redis-utils-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-04-14 11:38:37.535309 py-redis-utils-1.0.8/
--rw-r--r--   0 erne      (1000) erne      (1000)      478 2023-04-14 11:38:37.535309 py-redis-utils-1.0.8/PKG-INFO
--rwxrwxrwx   0 erne      (1000) erne      (1000)     1361 2023-02-03 14:24:27.000000 py-redis-utils-1.0.8/README.md
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-04-14 11:38:37.535309 py-redis-utils-1.0.8/py_redis_utils.egg-info/
--rw-r--r--   0 erne      (1000) erne      (1000)      478 2023-04-14 11:38:37.000000 py-redis-utils-1.0.8/py_redis_utils.egg-info/PKG-INFO
--rw-r--r--   0 erne      (1000) erne      (1000)      259 2023-04-14 11:38:37.000000 py-redis-utils-1.0.8/py_redis_utils.egg-info/SOURCES.txt
--rw-r--r--   0 erne      (1000) erne      (1000)        1 2023-04-14 11:38:37.000000 py-redis-utils-1.0.8/py_redis_utils.egg-info/dependency_links.txt
--rw-r--r--   0 erne      (1000) erne      (1000)       21 2023-04-14 11:38:37.000000 py-redis-utils-1.0.8/py_redis_utils.egg-info/requires.txt
--rw-r--r--   0 erne      (1000) erne      (1000)       13 2023-04-14 11:38:37.000000 py-redis-utils-1.0.8/py_redis_utils.egg-info/top_level.txt
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-04-14 11:38:37.535309 py-redis-utils-1.0.8/pyredisutils/
--rwxrwxrwx   0 erne      (1000) erne      (1000)       39 2023-02-03 12:53:24.000000 py-redis-utils-1.0.8/pyredisutils/__init__.py
--rw-r--r--   0 erne      (1000) erne      (1000)     6604 2023-04-14 11:37:15.000000 py-redis-utils-1.0.8/pyredisutils/_auth_deco.py
--rw-r--r--   0 erne      (1000) erne      (1000)       38 2023-04-14 11:38:37.535309 py-redis-utils-1.0.8/setup.cfg
--rw-r--r--   0 erne      (1000) erne      (1000)      696 2023-04-14 11:37:45.000000 py-redis-utils-1.0.8/setup.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-05-17 08:56:44.830864 py-redis-utils-1.0.9/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      416 2023-05-17 08:56:44.830864 py-redis-utils-1.0.9/PKG-INFO
+-rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)     1361 2023-04-11 16:05:30.000000 py-redis-utils-1.0.9/README.md
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-05-17 08:56:44.830864 py-redis-utils-1.0.9/py_redis_utils.egg-info/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      416 2023-05-17 08:56:44.000000 py-redis-utils-1.0.9/py_redis_utils.egg-info/PKG-INFO
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      286 2023-05-17 08:56:44.000000 py-redis-utils-1.0.9/py_redis_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)        1 2023-05-17 08:56:44.000000 py-redis-utils-1.0.9/py_redis_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       63 2023-05-17 08:56:44.000000 py-redis-utils-1.0.9/py_redis_utils.egg-info/requires.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       13 2023-05-17 08:56:44.000000 py-redis-utils-1.0.9/py_redis_utils.egg-info/top_level.txt
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-05-17 08:56:44.830864 py-redis-utils-1.0.9/pyredisutils/
+-rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)       65 2023-05-12 12:29:04.000000 py-redis-utils-1.0.9/pyredisutils/__init__.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)     8076 2023-05-12 13:03:07.000000 py-redis-utils-1.0.9/pyredisutils/_decorators.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)    14305 2023-05-17 08:41:59.000000 py-redis-utils-1.0.9/pyredisutils/_settings.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-05-17 08:56:44.830864 py-redis-utils-1.0.9/setup.cfg
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      786 2023-05-17 08:52:39.000000 py-redis-utils-1.0.9/setup.py
```

### Comparing `py-redis-utils-1.0.8/README.md` & `py-redis-utils-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `py-redis-utils-1.0.8/setup.py` & `py-redis-utils-1.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from setuptools import setup, find_packages
 
-VERSION = "1.0.8"
+VERSION = "1.0.9"
 DESCRIPTION = "Utilities with Redis"
 
 # Setting up
 setup(
     name="py-redis-utils",
     version=VERSION,
     author="KE",
     author_email="",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
-    install_requires=["flask", "redis", "deepdiff"],
-    keywords=["python", "flask", "JWT", "decorator", "token"],
+    install_requires=[
+        "flask>=2.0.0,<=2.2.3",
+        "redis>=4.5.0",
+        "deepdiff>=6.2.1",
+        "PyJWT>=2.0.0"
+    ],
+    keywords=["python", "flask", "PyJWT", "decorator", "token"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.11",
         "Operating System :: Unix",
         "Operating System :: MacOS",
     ],
```

