# Comparing `tmp/pubcontrol-3.3.0.tar.gz` & `tmp/pubcontrol-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pubcontrol-3.3.0.tar", last modified: Fri Apr 22 01:30:58 2022, max compression
+gzip compressed data, was "pubcontrol-3.4.0.tar", last modified: Wed May 17 19:21:30 2023, max compression
```

## Comparing `pubcontrol-3.3.0.tar` & `pubcontrol-3.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jkarneges   (501) staff       (20)        0 2022-04-22 01:30:58.347457 pubcontrol-3.3.0/
--rw-r--r--   0 jkarneges   (501) staff       (20)     1056 2022-04-22 01:30:17.000000 pubcontrol-3.3.0/COPYING
--rw-r--r--   0 jkarneges   (501) staff       (20)      326 2022-04-22 01:30:58.347024 pubcontrol-3.3.0/PKG-INFO
--rw-r--r--   0 jkarneges   (501) staff       (20)     4331 2022-04-22 01:30:17.000000 pubcontrol-3.3.0/README.md
-drwxr-xr-x   0 jkarneges   (501) staff       (20)        0 2022-04-22 01:30:58.341165 pubcontrol-3.3.0/pubcontrol.egg-info/
--rw-r--r--   0 jkarneges   (501) staff       (20)      326 2022-04-22 01:30:57.000000 pubcontrol-3.3.0/pubcontrol.egg-info/PKG-INFO
--rw-r--r--   0 jkarneges   (501) staff       (20)      388 2022-04-22 01:30:58.000000 pubcontrol-3.3.0/pubcontrol.egg-info/SOURCES.txt
--rw-r--r--   0 jkarneges   (501) staff       (20)        1 2022-04-22 01:30:57.000000 pubcontrol-3.3.0/pubcontrol.egg-info/dependency_links.txt
--rw-r--r--   0 jkarneges   (501) staff       (20)       96 2022-04-22 01:30:58.000000 pubcontrol-3.3.0/pubcontrol.egg-info/requires.txt
--rw-r--r--   0 jkarneges   (501) staff       (20)       11 2022-04-22 01:30:58.000000 pubcontrol-3.3.0/pubcontrol.egg-info/top_level.txt
--rw-r--r--   0 jkarneges   (501) staff       (20)       38 2022-04-22 01:30:58.347669 pubcontrol-3.3.0/setup.cfg
--rw-r--r--   0 jkarneges   (501) staff       (20)      522 2022-04-22 01:30:17.000000 pubcontrol-3.3.0/setup.py
-drwxr-xr-x   0 jkarneges   (501) staff       (20)        0 2022-04-22 01:30:58.346217 pubcontrol-3.3.0/src/
--rw-r--r--   0 jkarneges   (501) staff       (20)      569 2022-04-22 01:30:17.000000 pubcontrol-3.3.0/src/__init__.py
--rw-r--r--   0 jkarneges   (501) staff       (20)      716 2022-04-22 01:30:17.000000 pubcontrol-3.3.0/src/format.py
--rw-r--r--   0 jkarneges   (501) staff       (20)     2420 2022-04-22 01:30:17.000000 pubcontrol-3.3.0/src/item.py
--rw-r--r--   0 jkarneges   (501) staff       (20)     1846 2022-04-22 01:30:17.000000 pubcontrol-3.3.0/src/pcccbhandler.py
--rw-r--r--   0 jkarneges   (501) staff       (20)    11448 2022-04-22 01:30:17.000000 pubcontrol-3.3.0/src/pubcontrol.py
--rw-r--r--   0 jkarneges   (501) staff       (20)    10349 2022-04-22 01:30:17.000000 pubcontrol-3.3.0/src/pubcontrolclient.py
--rw-r--r--   0 jkarneges   (501) staff       (20)    10369 2022-04-22 01:30:17.000000 pubcontrol-3.3.0/src/pubsubmonitor.py
--rw-r--r--   0 jkarneges   (501) staff       (20)     2414 2022-04-22 01:30:17.000000 pubcontrol-3.3.0/src/utilities.py
--rw-r--r--   0 jkarneges   (501) staff       (20)    12981 2022-04-22 01:30:17.000000 pubcontrol-3.3.0/src/zmqpubcontrolclient.py
--rw-r--r--   0 jkarneges   (501) staff       (20)     6432 2022-04-22 01:30:17.000000 pubcontrol-3.3.0/src/zmqpubcontroller.py
+drwxr-xr-x   0 jkarneges   (501) staff       (20)        0 2023-05-17 19:21:30.728363 pubcontrol-3.4.0/
+-rw-r--r--   0 jkarneges   (501) staff       (20)     1056 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/COPYING
+-rw-r--r--   0 jkarneges   (501) staff       (20)      326 2023-05-17 19:21:30.727973 pubcontrol-3.4.0/PKG-INFO
+-rw-r--r--   0 jkarneges   (501) staff       (20)     4331 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/README.md
+drwxr-xr-x   0 jkarneges   (501) staff       (20)        0 2023-05-17 19:21:30.720433 pubcontrol-3.4.0/pubcontrol.egg-info/
+-rw-r--r--   0 jkarneges   (501) staff       (20)      326 2023-05-17 19:21:30.000000 pubcontrol-3.4.0/pubcontrol.egg-info/PKG-INFO
+-rw-r--r--   0 jkarneges   (501) staff       (20)      388 2023-05-17 19:21:30.000000 pubcontrol-3.4.0/pubcontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 jkarneges   (501) staff       (20)        1 2023-05-17 19:21:30.000000 pubcontrol-3.4.0/pubcontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 jkarneges   (501) staff       (20)       96 2023-05-17 19:21:30.000000 pubcontrol-3.4.0/pubcontrol.egg-info/requires.txt
+-rw-r--r--   0 jkarneges   (501) staff       (20)       11 2023-05-17 19:21:30.000000 pubcontrol-3.4.0/pubcontrol.egg-info/top_level.txt
+-rw-r--r--   0 jkarneges   (501) staff       (20)       38 2023-05-17 19:21:30.728496 pubcontrol-3.4.0/setup.cfg
+-rw-r--r--   0 jkarneges   (501) staff       (20)      522 2023-05-17 19:21:17.000000 pubcontrol-3.4.0/setup.py
+drwxr-xr-x   0 jkarneges   (501) staff       (20)        0 2023-05-17 19:21:30.726932 pubcontrol-3.4.0/src/
+-rw-r--r--   0 jkarneges   (501) staff       (20)      569 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/src/__init__.py
+-rw-r--r--   0 jkarneges   (501) staff       (20)      716 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/src/format.py
+-rw-r--r--   0 jkarneges   (501) staff       (20)     2420 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/src/item.py
+-rw-r--r--   0 jkarneges   (501) staff       (20)     1846 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/src/pcccbhandler.py
+-rw-r--r--   0 jkarneges   (501) staff       (20)    11448 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/src/pubcontrol.py
+-rw-r--r--   0 jkarneges   (501) staff       (20)    10348 2023-05-17 19:21:17.000000 pubcontrol-3.4.0/src/pubcontrolclient.py
+-rw-r--r--   0 jkarneges   (501) staff       (20)    10369 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/src/pubsubmonitor.py
+-rw-r--r--   0 jkarneges   (501) staff       (20)     2414 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/src/utilities.py
+-rw-r--r--   0 jkarneges   (501) staff       (20)    12981 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/src/zmqpubcontrolclient.py
+-rw-r--r--   0 jkarneges   (501) staff       (20)     6432 2022-04-22 01:30:17.000000 pubcontrol-3.4.0/src/zmqpubcontroller.py
```

### Comparing `pubcontrol-3.3.0/COPYING` & `pubcontrol-3.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `pubcontrol-3.3.0/README.md` & `pubcontrol-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pubcontrol-3.3.0/setup.py` & `pubcontrol-3.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(
 	name='pubcontrol',
-	version='3.3.0',
+	version='3.4.0',
 	description='EPCP library',
 	author='Justin Karneges',
 	author_email='justin@fanout.io',
 	url='https://github.com/fanout/pypubcontrol',
 	license='MIT',
 	package_dir={'pubcontrol': 'src'},
 	packages=['pubcontrol'],
```

### Comparing `pubcontrol-3.3.0/src/__init__.py` & `pubcontrol-3.4.0/src/__init__.py`

 * *Files identical despite different names*

### Comparing `pubcontrol-3.3.0/src/format.py` & `pubcontrol-3.4.0/src/format.py`

 * *Files identical despite different names*

### Comparing `pubcontrol-3.3.0/src/item.py` & `pubcontrol-3.4.0/src/item.py`

 * *Files identical despite different names*

### Comparing `pubcontrol-3.3.0/src/pcccbhandler.py` & `pubcontrol-3.4.0/src/pcccbhandler.py`

 * *Files identical despite different names*

### Comparing `pubcontrol-3.3.0/src/pubcontrol.py` & `pubcontrol-3.4.0/src/pubcontrol.py`

 * *Files identical despite different names*

### Comparing `pubcontrol-3.3.0/src/pubcontrolclient.py` & `pubcontrol-3.4.0/src/pubcontrolclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 		self.sub_monitor = None
 		self.closed = False
 
 		retry = Retry(
 			total=1,
 			backoff_factor=0.5,
 			status_forcelist=[500, 502, 503, 504],
-			method_whitelist=frozenset(['GET', 'POST'])
+			allowed_methods=frozenset(['GET', 'POST'])
 		)
 
 		adapter = HTTPAdapter(max_retries=retry)
 
 		self.requests_session = requests.session()
 		self.requests_session.mount('http://', adapter)
 		self.requests_session.mount('https://', adapter)
```

### Comparing `pubcontrol-3.3.0/src/pubsubmonitor.py` & `pubcontrol-3.4.0/src/pubsubmonitor.py`

 * *Files identical despite different names*

### Comparing `pubcontrol-3.3.0/src/utilities.py` & `pubcontrol-3.4.0/src/utilities.py`

 * *Files identical despite different names*

### Comparing `pubcontrol-3.3.0/src/zmqpubcontrolclient.py` & `pubcontrol-3.4.0/src/zmqpubcontrolclient.py`

 * *Files identical despite different names*

### Comparing `pubcontrol-3.3.0/src/zmqpubcontroller.py` & `pubcontrol-3.4.0/src/zmqpubcontroller.py`

 * *Files identical despite different names*

