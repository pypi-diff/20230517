# Comparing `tmp/asyncactor-0.23.1.tar.gz` & `tmp/asyncactor-0.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncactor-0.23.1.tar", last modified: Fri Sep 16 17:50:54 2022, max compression
+gzip compressed data, was "asyncactor-0.24.0.tar", last modified: Wed May 17 15:24:24 2023, max compression
```

## Comparing `asyncactor-0.23.1.tar` & `asyncactor-0.24.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-16 17:50:54.956552 asyncactor-0.23.1/
--rw-r--r--   0 smurf      (501) smurf      (501)       49 2019-09-27 14:05:18.000000 asyncactor-0.23.1/.coveragerc
--rw-r--r--   0 smurf      (501) smurf      (501)      543 2019-10-02 17:17:45.000000 asyncactor-0.23.1/.gitignore
--rw-r--r--   0 smurf      (501) smurf      (501)      151 2020-07-29 11:54:57.000000 asyncactor-0.23.1/.pylintrc
--rw-r--r--   0 smurf      (501) smurf      (501)      173 2019-09-27 14:05:18.000000 asyncactor-0.23.1/.readthedocs.yml
--rw-r--r--   0 smurf      (501) smurf      (501)     5373 2019-09-27 14:05:18.000000 asyncactor-0.23.1/.style.yapf
--rw-r--r--   0 smurf      (501) smurf      (501)      834 2019-09-27 14:05:18.000000 asyncactor-0.23.1/.travis.yml
--rw-r--r--   0 smurf      (501) smurf      (501)      154 2020-01-29 16:30:28.000000 asyncactor-0.23.1/CHANGELOG.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     1114 2019-09-27 14:05:18.000000 asyncactor-0.23.1/LICENSE
--rw-r--r--   0 smurf      (501) smurf      (501)      243 2020-07-29 11:54:57.000000 asyncactor-0.23.1/Makefile
--rw-r--r--   0 smurf      (501) smurf      (501)     3442 2022-09-16 17:50:54.956552 asyncactor-0.23.1/PKG-INFO
--rw-r--r--   0 smurf      (501) smurf      (501)     3059 2022-09-13 07:11:51.000000 asyncactor-0.23.1/README.rst
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-16 17:50:54.956552 asyncactor-0.23.1/asyncactor/
--rw-r--r--   0 smurf      (501) smurf      (501)      305 2020-07-29 11:54:57.000000 asyncactor-0.23.1/asyncactor/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1296 2020-07-29 11:54:57.000000 asyncactor-0.23.1/asyncactor/abc.py
--rw-r--r--   0 smurf      (501) smurf      (501)    27262 2022-09-16 17:47:59.000000 asyncactor-0.23.1/asyncactor/actor.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-16 17:50:54.956552 asyncactor-0.23.1/asyncactor/backend/
--rw-r--r--   0 smurf      (501) smurf      (501)      175 2020-07-29 11:54:57.000000 asyncactor-0.23.1/asyncactor/backend/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1414 2020-08-27 07:36:44.000000 asyncactor-0.23.1/asyncactor/backend/distkv.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2171 2022-09-16 17:46:14.000000 asyncactor-0.23.1/asyncactor/backend/mqtt.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1319 2020-08-27 07:36:44.000000 asyncactor-0.23.1/asyncactor/backend/serf.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4012 2020-07-29 14:42:17.000000 asyncactor-0.23.1/asyncactor/events.py
--rw-r--r--   0 smurf      (501) smurf      (501)      352 2019-10-02 16:49:00.000000 asyncactor-0.23.1/asyncactor/exceptions.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2904 2020-09-07 07:27:36.000000 asyncactor-0.23.1/asyncactor/messages.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2204 2020-08-27 07:36:44.000000 asyncactor-0.23.1/asyncactor/nodelist.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-16 17:50:54.956552 asyncactor-0.23.1/asyncactor.egg-info/
--rw-r--r--   0 smurf      (501) smurf      (501)     3442 2022-09-16 17:50:54.000000 asyncactor-0.23.1/asyncactor.egg-info/PKG-INFO
--rw-r--r--   0 smurf      (501) smurf      (501)      919 2022-09-16 17:50:54.000000 asyncactor-0.23.1/asyncactor.egg-info/SOURCES.txt
--rw-r--r--   0 smurf      (501) smurf      (501)        1 2022-09-16 17:50:54.000000 asyncactor-0.23.1/asyncactor.egg-info/dependency_links.txt
--rw-r--r--   0 smurf      (501) smurf      (501)      104 2022-09-16 17:50:54.000000 asyncactor-0.23.1/asyncactor.egg-info/requires.txt
--rw-r--r--   0 smurf      (501) smurf      (501)       17 2022-09-16 17:50:54.000000 asyncactor-0.23.1/asyncactor.egg-info/top_level.txt
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-16 17:50:54.956552 asyncactor-0.23.1/ci/
--rw-r--r--   0 smurf      (501) smurf      (501)       52 2019-09-27 14:05:18.000000 asyncactor-0.23.1/ci/rtd-requirements.txt
--rw-r--r--   0 smurf      (501) smurf      (501)       55 2019-09-27 14:05:18.000000 asyncactor-0.23.1/ci/test-requirements.txt
--rwxr-xr-x   0 smurf      (501) smurf      (501)     3421 2019-10-02 16:49:00.000000 asyncactor-0.23.1/ci/travis.sh
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-16 17:50:54.956552 asyncactor-0.23.1/docs/
--rw-r--r--   0 smurf      (501) smurf      (501)      612 2019-10-02 16:49:00.000000 asyncactor-0.23.1/docs/Makefile
--rw-r--r--   0 smurf      (501) smurf      (501)      782 2019-10-02 16:49:00.000000 asyncactor-0.23.1/docs/make.bat
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-16 17:50:54.956552 asyncactor-0.23.1/docs/source/
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-16 17:50:54.956552 asyncactor-0.23.1/docs/source/_static/
--rw-r--r--   0 smurf      (501) smurf      (501)        0 2019-09-27 14:05:18.000000 asyncactor-0.23.1/docs/source/_static/.git_empty
--rw-r--r--   0 smurf      (501) smurf      (501)     5127 2020-01-29 20:03:47.000000 asyncactor-0.23.1/docs/source/actor.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     6125 2019-10-02 16:49:00.000000 asyncactor-0.23.1/docs/source/conf.py
--rw-r--r--   0 smurf      (501) smurf      (501)      154 2019-10-02 16:49:00.000000 asyncactor-0.23.1/docs/source/history.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     1162 2019-10-02 16:49:00.000000 asyncactor-0.23.1/docs/source/index.rst
--rw-r--r--   0 smurf      (501) smurf      (501)      316 2019-10-02 16:49:00.000000 asyncactor-0.23.1/docs/source/rationale.rst
--rwxr-xr-x   0 smurf      (501) smurf      (501)      195 2019-09-27 14:05:18.000000 asyncactor-0.23.1/mktag
--rw-r--r--   0 smurf      (501) smurf      (501)      267 2022-09-16 17:50:54.956552 asyncactor-0.23.1/setup.cfg
--rw-r--r--   0 smurf      (501) smurf      (501)     1640 2022-09-16 17:46:22.000000 asyncactor-0.23.1/setup.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2022-09-16 17:50:54.956552 asyncactor-0.23.1/tests/
--rw-r--r--   0 smurf      (501) smurf      (501)      226 2019-09-27 14:05:18.000000 asyncactor-0.23.1/tests/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3769 2022-09-16 17:46:31.000000 asyncactor-0.23.1/tests/mock_serf.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5009 2020-08-27 07:36:44.000000 asyncactor-0.23.1/tests/test_actor.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4071 2022-09-16 17:46:41.000000 asyncactor-0.23.1/tests/test_mosquitto.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3628 2020-08-27 07:36:44.000000 asyncactor-0.23.1/tests/test_serf.py
--rw-r--r--   0 smurf      (501) smurf      (501)      207 2019-10-02 16:49:00.000000 asyncactor-0.23.1/tox.ini
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-17 15:24:24.027884 asyncactor-0.24.0/
+-rw-r--r--   0 smurf      (501) smurf      (501)       49 2019-09-27 14:05:18.000000 asyncactor-0.24.0/.coveragerc
+-rw-r--r--   0 smurf      (501) smurf      (501)      552 2023-05-17 15:24:22.000000 asyncactor-0.24.0/.gitignore
+-rw-r--r--   0 smurf      (501) smurf      (501)      151 2020-07-29 11:54:57.000000 asyncactor-0.24.0/.pylintrc
+-rw-r--r--   0 smurf      (501) smurf      (501)      173 2019-09-27 14:05:18.000000 asyncactor-0.24.0/.readthedocs.yml
+-rw-r--r--   0 smurf      (501) smurf      (501)     5373 2019-09-27 14:05:18.000000 asyncactor-0.24.0/.style.yapf
+-rw-r--r--   0 smurf      (501) smurf      (501)      834 2019-09-27 14:05:18.000000 asyncactor-0.24.0/.travis.yml
+-rw-r--r--   0 smurf      (501) smurf      (501)      154 2020-01-29 16:30:28.000000 asyncactor-0.24.0/CHANGELOG.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     1114 2019-09-27 14:05:18.000000 asyncactor-0.24.0/LICENSE
+-rw-r--r--   0 smurf      (501) smurf      (501)      243 2020-07-29 11:54:57.000000 asyncactor-0.24.0/Makefile
+-rw-r--r--   0 smurf      (501) smurf      (501)     3442 2023-05-17 15:24:24.027884 asyncactor-0.24.0/PKG-INFO
+-rw-r--r--   0 smurf      (501) smurf      (501)     3059 2022-09-22 13:17:11.000000 asyncactor-0.24.0/README.rst
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-17 15:24:24.023883 asyncactor-0.24.0/asyncactor/
+-rw-r--r--   0 smurf      (501) smurf      (501)      305 2020-07-29 11:54:57.000000 asyncactor-0.24.0/asyncactor/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1296 2020-07-29 11:54:57.000000 asyncactor-0.24.0/asyncactor/abc.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    27262 2023-04-25 16:59:08.000000 asyncactor-0.24.0/asyncactor/actor.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-17 15:24:24.023883 asyncactor-0.24.0/asyncactor/backend/
+-rw-r--r--   0 smurf      (501) smurf      (501)      175 2020-07-29 11:54:57.000000 asyncactor-0.24.0/asyncactor/backend/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1414 2020-08-27 07:36:44.000000 asyncactor-0.24.0/asyncactor/backend/distkv.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1383 2023-05-17 15:24:00.000000 asyncactor-0.24.0/asyncactor/backend/moat_kv.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2171 2022-09-22 13:17:11.000000 asyncactor-0.24.0/asyncactor/backend/mqtt.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1319 2020-08-27 07:36:44.000000 asyncactor-0.24.0/asyncactor/backend/serf.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4012 2020-07-29 14:42:17.000000 asyncactor-0.24.0/asyncactor/events.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      352 2019-10-02 16:49:00.000000 asyncactor-0.24.0/asyncactor/exceptions.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2904 2020-09-07 07:27:36.000000 asyncactor-0.24.0/asyncactor/messages.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2204 2020-08-27 07:36:44.000000 asyncactor-0.24.0/asyncactor/nodelist.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-17 15:24:24.023883 asyncactor-0.24.0/asyncactor.egg-info/
+-rw-r--r--   0 smurf      (501) smurf      (501)     3442 2023-05-17 15:24:23.000000 asyncactor-0.24.0/asyncactor.egg-info/PKG-INFO
+-rw-r--r--   0 smurf      (501) smurf      (501)      949 2023-05-17 15:24:23.000000 asyncactor-0.24.0/asyncactor.egg-info/SOURCES.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)        1 2023-05-17 15:24:23.000000 asyncactor-0.24.0/asyncactor.egg-info/dependency_links.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)      104 2023-05-17 15:24:23.000000 asyncactor-0.24.0/asyncactor.egg-info/requires.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)       17 2023-05-17 15:24:23.000000 asyncactor-0.24.0/asyncactor.egg-info/top_level.txt
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-17 15:24:24.023883 asyncactor-0.24.0/ci/
+-rw-r--r--   0 smurf      (501) smurf      (501)       52 2019-09-27 14:05:18.000000 asyncactor-0.24.0/ci/rtd-requirements.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)       55 2019-09-27 14:05:18.000000 asyncactor-0.24.0/ci/test-requirements.txt
+-rwxr-xr-x   0 smurf      (501) smurf      (501)     3421 2019-10-02 16:49:00.000000 asyncactor-0.24.0/ci/travis.sh
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-17 15:24:24.023883 asyncactor-0.24.0/docs/
+-rw-r--r--   0 smurf      (501) smurf      (501)      612 2019-10-02 16:49:00.000000 asyncactor-0.24.0/docs/Makefile
+-rw-r--r--   0 smurf      (501) smurf      (501)      782 2019-10-02 16:49:00.000000 asyncactor-0.24.0/docs/make.bat
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-17 15:24:24.023883 asyncactor-0.24.0/docs/source/
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-17 15:24:24.027884 asyncactor-0.24.0/docs/source/_static/
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2019-09-27 14:05:18.000000 asyncactor-0.24.0/docs/source/_static/.git_empty
+-rw-r--r--   0 smurf      (501) smurf      (501)     5127 2020-01-29 20:03:47.000000 asyncactor-0.24.0/docs/source/actor.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     6125 2019-10-02 16:49:00.000000 asyncactor-0.24.0/docs/source/conf.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      154 2019-10-02 16:49:00.000000 asyncactor-0.24.0/docs/source/history.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     1162 2019-10-02 16:49:00.000000 asyncactor-0.24.0/docs/source/index.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)      316 2019-10-02 16:49:00.000000 asyncactor-0.24.0/docs/source/rationale.rst
+-rwxr-xr-x   0 smurf      (501) smurf      (501)      195 2019-09-27 14:05:18.000000 asyncactor-0.24.0/mktag
+-rw-r--r--   0 smurf      (501) smurf      (501)      267 2023-05-17 15:24:24.027884 asyncactor-0.24.0/setup.cfg
+-rw-r--r--   0 smurf      (501) smurf      (501)     1640 2022-09-22 13:17:11.000000 asyncactor-0.24.0/setup.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-17 15:24:24.027884 asyncactor-0.24.0/tests/
+-rw-r--r--   0 smurf      (501) smurf      (501)      226 2019-09-27 14:05:18.000000 asyncactor-0.24.0/tests/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3769 2022-09-22 13:17:11.000000 asyncactor-0.24.0/tests/mock_serf.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5009 2020-08-27 07:36:44.000000 asyncactor-0.24.0/tests/test_actor.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4071 2022-09-22 13:17:11.000000 asyncactor-0.24.0/tests/test_mosquitto.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3628 2020-08-27 07:36:44.000000 asyncactor-0.24.0/tests/test_serf.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      207 2019-10-02 16:49:00.000000 asyncactor-0.24.0/tox.ini
```

### Comparing `asyncactor-0.23.1/.gitignore` & `asyncactor-0.24.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -45,7 +45,8 @@
 [._]s[a-w][a-z]
 *.un~
 *~
 /.pybuild
 
 # local stuff
 /T
+/debian/
```

### Comparing `asyncactor-0.23.1/.style.yapf` & `asyncactor-0.24.0/.style.yapf`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/.travis.yml` & `asyncactor-0.24.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/LICENSE` & `asyncactor-0.24.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/PKG-INFO` & `asyncactor-0.24.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncactor
-Version: 0.23.1
+Version: 0.24.0
 Summary: Async decentralized actor
 Home-page: https://github.com/smurfix/asyncactor
 Author: Matthias Urlichs
 Author-email: matthias@urlichs.de
 Maintainer: Matthias Urlichs
 Maintainer-email: matthias@urlichs.de
 License: GPL3
```

### Comparing `asyncactor-0.23.1/README.rst` & `asyncactor-0.24.0/README.rst`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/asyncactor/abc.py` & `asyncactor-0.24.0/asyncactor/abc.py`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/asyncactor/actor.py` & `asyncactor-0.24.0/asyncactor/actor.py`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/asyncactor/backend/distkv.py` & `asyncactor-0.24.0/asyncactor/backend/distkv.py`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/asyncactor/backend/mqtt.py` & `asyncactor-0.24.0/asyncactor/backend/mqtt.py`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/asyncactor/backend/serf.py` & `asyncactor-0.24.0/asyncactor/backend/serf.py`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/asyncactor/events.py` & `asyncactor-0.24.0/asyncactor/events.py`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/asyncactor/messages.py` & `asyncactor-0.24.0/asyncactor/messages.py`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/asyncactor/nodelist.py` & `asyncactor-0.24.0/asyncactor/nodelist.py`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/asyncactor.egg-info/PKG-INFO` & `asyncactor-0.24.0/asyncactor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncactor
-Version: 0.23.1
+Version: 0.24.0
 Summary: Async decentralized actor
 Home-page: https://github.com/smurfix/asyncactor
 Author: Matthias Urlichs
 Author-email: matthias@urlichs.de
 Maintainer: Matthias Urlichs
 Maintainer-email: matthias@urlichs.de
 License: GPL3
```

### Comparing `asyncactor-0.23.1/asyncactor.egg-info/SOURCES.txt` & `asyncactor-0.24.0/asyncactor.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 asyncactor.egg-info/PKG-INFO
 asyncactor.egg-info/SOURCES.txt
 asyncactor.egg-info/dependency_links.txt
 asyncactor.egg-info/requires.txt
 asyncactor.egg-info/top_level.txt
 asyncactor/backend/__init__.py
 asyncactor/backend/distkv.py
+asyncactor/backend/moat_kv.py
 asyncactor/backend/mqtt.py
 asyncactor/backend/serf.py
 ci/rtd-requirements.txt
 ci/test-requirements.txt
 ci/travis.sh
 docs/Makefile
 docs/make.bat
```

### Comparing `asyncactor-0.23.1/ci/travis.sh` & `asyncactor-0.24.0/ci/travis.sh`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/docs/Makefile` & `asyncactor-0.24.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/docs/make.bat` & `asyncactor-0.24.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/docs/source/actor.rst` & `asyncactor-0.24.0/docs/source/actor.rst`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/docs/source/conf.py` & `asyncactor-0.24.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/docs/source/index.rst` & `asyncactor-0.24.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/setup.py` & `asyncactor-0.24.0/setup.py`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/tests/mock_serf.py` & `asyncactor-0.24.0/tests/mock_serf.py`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/tests/test_actor.py` & `asyncactor-0.24.0/tests/test_actor.py`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/tests/test_mosquitto.py` & `asyncactor-0.24.0/tests/test_mosquitto.py`

 * *Files identical despite different names*

### Comparing `asyncactor-0.23.1/tests/test_serf.py` & `asyncactor-0.24.0/tests/test_serf.py`

 * *Files identical despite different names*

