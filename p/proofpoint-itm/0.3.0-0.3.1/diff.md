# Comparing `tmp/proofpoint_itm-0.3.0.tar.gz` & `tmp/proofpoint_itm-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proofpoint_itm-0.3.0.tar", last modified: Tue Dec 13 22:33:39 2022, max compression
+gzip compressed data, was "proofpoint_itm-0.3.1.tar", last modified: Thu Dec 15 01:02:42 2022, max compression
```

## Comparing `proofpoint_itm-0.3.0.tar` & `proofpoint_itm-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 molden     (501) staff       (20)        0 2022-12-13 22:33:39.378113 proofpoint_itm-0.3.0/
--rw-r--r--   0 molden     (501) staff       (20)    11357 2021-11-16 02:23:49.000000 proofpoint_itm-0.3.0/LICENSE
--rw-r--r--   0 molden     (501) staff       (20)     8789 2022-12-13 22:33:39.378191 proofpoint_itm-0.3.0/PKG-INFO
--rw-r--r--   0 molden     (501) staff       (20)     8184 2022-12-11 05:38:51.000000 proofpoint_itm-0.3.0/README.md
--rw-r--r--   0 molden     (501) staff       (20)       74 2022-12-13 22:33:39.378442 proofpoint_itm-0.3.0/setup.cfg
--rw-r--r--   0 molden     (501) staff       (20)      933 2022-12-13 22:33:20.000000 proofpoint_itm-0.3.0/setup.py
-drwxr-xr-x   0 molden     (501) staff       (20)        0 2022-12-13 22:33:39.374942 proofpoint_itm-0.3.0/src/
-drwxr-xr-x   0 molden     (501) staff       (20)        0 2022-12-13 22:33:39.377359 proofpoint_itm-0.3.0/src/proofpoint_itm/
--rw-r--r--   0 molden     (501) staff       (20)       43 2022-10-14 21:09:35.000000 proofpoint_itm-0.3.0/src/proofpoint_itm/__init__.py
--rw-r--r--   0 molden     (501) staff       (20)     1359 2022-11-23 17:14:39.000000 proofpoint_itm-0.3.0/src/proofpoint_itm/auth.py
--rw-r--r--   0 molden     (501) staff       (20)    10810 2022-12-13 03:20:50.000000 proofpoint_itm-0.3.0/src/proofpoint_itm/classes.py
--rw-r--r--   0 molden     (501) staff       (20)    39118 2022-12-13 22:29:13.000000 proofpoint_itm-0.3.0/src/proofpoint_itm/client.py
--rw-r--r--   0 molden     (501) staff       (20)     2407 2022-11-23 17:14:48.000000 proofpoint_itm-0.3.0/src/proofpoint_itm/webclient.py
-drwxr-xr-x   0 molden     (501) staff       (20)        0 2022-12-13 22:33:39.378013 proofpoint_itm-0.3.0/src/proofpoint_itm.egg-info/
--rw-r--r--   0 molden     (501) staff       (20)     8789 2022-12-13 22:33:39.000000 proofpoint_itm-0.3.0/src/proofpoint_itm.egg-info/PKG-INFO
--rw-r--r--   0 molden     (501) staff       (20)      394 2022-12-13 22:33:39.000000 proofpoint_itm-0.3.0/src/proofpoint_itm.egg-info/SOURCES.txt
--rw-r--r--   0 molden     (501) staff       (20)        1 2022-12-13 22:33:39.000000 proofpoint_itm-0.3.0/src/proofpoint_itm.egg-info/dependency_links.txt
--rw-r--r--   0 molden     (501) staff       (20)        9 2022-12-13 22:33:39.000000 proofpoint_itm-0.3.0/src/proofpoint_itm.egg-info/requires.txt
--rw-r--r--   0 molden     (501) staff       (20)       15 2022-12-13 22:33:39.000000 proofpoint_itm-0.3.0/src/proofpoint_itm.egg-info/top_level.txt
+drwxr-xr-x   0 molden     (501) staff       (20)        0 2022-12-15 01:02:42.464215 proofpoint_itm-0.3.1/
+-rw-r--r--   0 molden     (501) staff       (20)    11357 2021-11-16 02:23:49.000000 proofpoint_itm-0.3.1/LICENSE
+-rw-r--r--   0 molden     (501) staff       (20)     8804 2022-12-15 01:02:42.464278 proofpoint_itm-0.3.1/PKG-INFO
+-rw-r--r--   0 molden     (501) staff       (20)     8184 2022-12-11 05:38:51.000000 proofpoint_itm-0.3.1/README.md
+-rw-r--r--   0 molden     (501) staff       (20)       74 2022-12-15 01:02:42.464529 proofpoint_itm-0.3.1/setup.cfg
+-rw-r--r--   0 molden     (501) staff       (20)      925 2022-12-15 01:02:00.000000 proofpoint_itm-0.3.1/setup.py
+drwxr-xr-x   0 molden     (501) staff       (20)        0 2022-12-15 01:02:42.462401 proofpoint_itm-0.3.1/src/
+drwxr-xr-x   0 molden     (501) staff       (20)        0 2022-12-15 01:02:42.463555 proofpoint_itm-0.3.1/src/proofpoint_itm/
+-rw-r--r--   0 molden     (501) staff       (20)       43 2022-10-14 21:09:35.000000 proofpoint_itm-0.3.1/src/proofpoint_itm/__init__.py
+-rw-r--r--   0 molden     (501) staff       (20)     1359 2022-11-23 17:14:39.000000 proofpoint_itm-0.3.1/src/proofpoint_itm/auth.py
+-rw-r--r--   0 molden     (501) staff       (20)    10810 2022-12-13 03:20:50.000000 proofpoint_itm-0.3.1/src/proofpoint_itm/classes.py
+-rw-r--r--   0 molden     (501) staff       (20)    39118 2022-12-13 22:29:13.000000 proofpoint_itm-0.3.1/src/proofpoint_itm/client.py
+-rw-r--r--   0 molden     (501) staff       (20)     2407 2022-11-23 17:14:48.000000 proofpoint_itm-0.3.1/src/proofpoint_itm/webclient.py
+drwxr-xr-x   0 molden     (501) staff       (20)        0 2022-12-15 01:02:42.464102 proofpoint_itm-0.3.1/src/proofpoint_itm.egg-info/
+-rw-r--r--   0 molden     (501) staff       (20)     8804 2022-12-15 01:02:42.000000 proofpoint_itm-0.3.1/src/proofpoint_itm.egg-info/PKG-INFO
+-rw-r--r--   0 molden     (501) staff       (20)      353 2022-12-15 01:02:42.000000 proofpoint_itm-0.3.1/src/proofpoint_itm.egg-info/SOURCES.txt
+-rw-r--r--   0 molden     (501) staff       (20)        1 2022-12-15 01:02:42.000000 proofpoint_itm-0.3.1/src/proofpoint_itm.egg-info/dependency_links.txt
+-rw-r--r--   0 molden     (501) staff       (20)       15 2022-12-15 01:02:42.000000 proofpoint_itm-0.3.1/src/proofpoint_itm.egg-info/top_level.txt
```

### Comparing `proofpoint_itm-0.3.0/LICENSE` & `proofpoint_itm-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proofpoint_itm-0.3.0/PKG-INFO` & `proofpoint_itm-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: proofpoint_itm
-Version: 0.3.0
+Version: 0.3.1
 Summary: Proofpoint ITM API client library
 Home-page: https://github.com/drizzo-tech/proofpoint_itm
 Author: Mike Olden
 Author-email: michael.olden@oldendigital.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/drizzo-tech/proofpoint_itm/issues
-Keywords: Proofpoint,ITM,ObserveIT
+Keywords: Proofpoint ITM,Proofpoint,ITM,ObserveIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `proofpoint_itm-0.3.0/README.md` & `proofpoint_itm-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `proofpoint_itm-0.3.0/setup.py` & `proofpoint_itm-0.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(name='proofpoint_itm',
-    version='0.3.0',
+    version='0.3.1',
     description='Proofpoint ITM API client library',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='Mike Olden',
     author_email='michael.olden@oldendigital.com',
     url = 'https://github.com/drizzo-tech/proofpoint_itm',
     project_urls={
@@ -20,12 +20,10 @@
     'License :: OSI Approved :: Apache Software License',
     'Operating System :: OS Independent',
     ],
     license='Apache 2.0',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     python_requires='>=3.6, <4',
-    install_requires=[
-        'requests'
-    ],
-    keywords='Proofpoint, ITM, ObserveIT'
+    install_requires=[],
+    keywords='Proofpoint ITM, Proofpoint, ITM, ObserveIT'
 )
```

### Comparing `proofpoint_itm-0.3.0/src/proofpoint_itm/auth.py` & `proofpoint_itm-0.3.1/src/proofpoint_itm/auth.py`

 * *Files identical despite different names*

### Comparing `proofpoint_itm-0.3.0/src/proofpoint_itm/classes.py` & `proofpoint_itm-0.3.1/src/proofpoint_itm/classes.py`

 * *Files identical despite different names*

### Comparing `proofpoint_itm-0.3.0/src/proofpoint_itm/client.py` & `proofpoint_itm-0.3.1/src/proofpoint_itm/client.py`

 * *Files identical despite different names*

### Comparing `proofpoint_itm-0.3.0/src/proofpoint_itm/webclient.py` & `proofpoint_itm-0.3.1/src/proofpoint_itm/webclient.py`

 * *Files identical despite different names*

### Comparing `proofpoint_itm-0.3.0/src/proofpoint_itm.egg-info/PKG-INFO` & `proofpoint_itm-0.3.1/src/proofpoint_itm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: proofpoint-itm
-Version: 0.3.0
+Version: 0.3.1
 Summary: Proofpoint ITM API client library
 Home-page: https://github.com/drizzo-tech/proofpoint_itm
 Author: Mike Olden
 Author-email: michael.olden@oldendigital.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/drizzo-tech/proofpoint_itm/issues
-Keywords: Proofpoint,ITM,ObserveIT
+Keywords: Proofpoint ITM,Proofpoint,ITM,ObserveIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

