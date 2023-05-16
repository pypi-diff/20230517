# Comparing `tmp/rfmanalysis-0.1.4.tar.gz` & `tmp/rfmanalysis-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfmanalysis-0.1.4.tar", last modified: Tue May 16 22:12:42 2023, max compression
+gzip compressed data, was "rfmanalysis-0.1.5.tar", last modified: Tue May 16 22:17:59 2023, max compression
```

## Comparing `rfmanalysis-0.1.4.tar` & `rfmanalysis-0.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 22:12:42.385012 rfmanalysis-0.1.4/
--rw-rw-rw-   0        0        0      184 2023-05-16 18:36:44.000000 rfmanalysis-0.1.4/AUTHORS.rst
--rw-rw-rw-   0        0        0     3690 2023-05-16 18:36:44.000000 rfmanalysis-0.1.4/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-05-16 18:36:44.000000 rfmanalysis-0.1.4/HISTORY.rst
--rw-rw-rw-   0        0        0     1098 2023-05-16 18:36:44.000000 rfmanalysis-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      273 2023-05-16 18:36:44.000000 rfmanalysis-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     5269 2023-05-16 22:12:42.386012 rfmanalysis-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4105 2023-05-16 18:42:22.000000 rfmanalysis-0.1.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-16 22:12:42.339887 rfmanalysis-0.1.4/docs/
--rw-rw-rw-   0        0        0      632 2023-05-16 18:36:44.000000 rfmanalysis-0.1.4/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-05-16 18:36:44.000000 rfmanalysis-0.1.4/docs/authors.rst
--rw-rw-rw-   0        0        0     5007 2023-05-16 21:26:34.000000 rfmanalysis-0.1.4/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-05-16 18:36:44.000000 rfmanalysis-0.1.4/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-05-16 18:36:44.000000 rfmanalysis-0.1.4/docs/history.rst
--rw-rw-rw-   0        0        0      331 2023-05-16 18:36:44.000000 rfmanalysis-0.1.4/docs/index.rst
--rw-rw-rw-   0        0        0     1206 2023-05-16 18:36:44.000000 rfmanalysis-0.1.4/docs/installation.rst
--rwxrwxrwx   0        0        0      809 2023-05-16 18:36:44.000000 rfmanalysis-0.1.4/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-05-16 18:36:44.000000 rfmanalysis-0.1.4/docs/readme.rst
--rw-rw-rw-   0        0        0       87 2023-05-16 18:36:44.000000 rfmanalysis-0.1.4/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-05-16 22:12:42.344196 rfmanalysis-0.1.4/rfmanalysis/
--rw-rw-rw-   0        0        0      155 2023-05-16 22:10:26.000000 rfmanalysis-0.1.4/rfmanalysis/__init__.py
--rw-rw-rw-   0        0        0    10559 2023-05-16 16:19:14.000000 rfmanalysis-0.1.4/rfmanalysis/rfmanalysis.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:12:42.365224 rfmanalysis-0.1.4/rfmanalysis.egg-info/
--rw-rw-rw-   0        0        0     5269 2023-05-16 22:12:42.000000 rfmanalysis-0.1.4/rfmanalysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      524 2023-05-16 22:12:42.000000 rfmanalysis-0.1.4/rfmanalysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 22:12:42.000000 rfmanalysis-0.1.4/rfmanalysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-16 18:47:20.000000 rfmanalysis-0.1.4/rfmanalysis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-05-16 22:12:42.000000 rfmanalysis-0.1.4/rfmanalysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      454 2023-05-16 22:12:42.400915 rfmanalysis-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1658 2023-05-16 22:10:18.000000 rfmanalysis-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:12:42.380224 rfmanalysis-0.1.4/tests/
--rw-rw-rw-   0        0        0       42 2023-05-16 18:36:44.000000 rfmanalysis-0.1.4/tests/__init__.py
--rw-rw-rw-   0        0        0      589 2023-05-16 18:36:44.000000 rfmanalysis-0.1.4/tests/test_rfmanalysis.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:17:58.996369 rfmanalysis-0.1.5/
+-rw-rw-rw-   0        0        0      184 2023-05-16 18:36:44.000000 rfmanalysis-0.1.5/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3690 2023-05-16 18:36:44.000000 rfmanalysis-0.1.5/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-05-16 18:36:44.000000 rfmanalysis-0.1.5/HISTORY.rst
+-rw-rw-rw-   0        0        0     1098 2023-05-16 18:36:44.000000 rfmanalysis-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-05-16 18:36:44.000000 rfmanalysis-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     5269 2023-05-16 22:17:58.996589 rfmanalysis-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4105 2023-05-16 18:42:22.000000 rfmanalysis-0.1.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-16 22:17:58.970350 rfmanalysis-0.1.5/docs/
+-rw-rw-rw-   0        0        0      632 2023-05-16 18:36:44.000000 rfmanalysis-0.1.5/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-05-16 18:36:44.000000 rfmanalysis-0.1.5/docs/authors.rst
+-rw-rw-rw-   0        0        0     5007 2023-05-16 21:26:34.000000 rfmanalysis-0.1.5/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-05-16 18:36:44.000000 rfmanalysis-0.1.5/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-05-16 18:36:44.000000 rfmanalysis-0.1.5/docs/history.rst
+-rw-rw-rw-   0        0        0      331 2023-05-16 18:36:44.000000 rfmanalysis-0.1.5/docs/index.rst
+-rw-rw-rw-   0        0        0     1206 2023-05-16 18:36:44.000000 rfmanalysis-0.1.5/docs/installation.rst
+-rwxrwxrwx   0        0        0      809 2023-05-16 18:36:44.000000 rfmanalysis-0.1.5/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-05-16 18:36:44.000000 rfmanalysis-0.1.5/docs/readme.rst
+-rw-rw-rw-   0        0        0       87 2023-05-16 18:36:44.000000 rfmanalysis-0.1.5/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-05-16 22:17:58.976021 rfmanalysis-0.1.5/rfmanalysis/
+-rw-rw-rw-   0        0        0      205 2023-05-16 22:17:20.000000 rfmanalysis-0.1.5/rfmanalysis/__init__.py
+-rw-rw-rw-   0        0        0    10559 2023-05-16 16:19:14.000000 rfmanalysis-0.1.5/rfmanalysis/rfmanalysis.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:17:58.990675 rfmanalysis-0.1.5/rfmanalysis.egg-info/
+-rw-rw-rw-   0        0        0     5269 2023-05-16 22:17:58.000000 rfmanalysis-0.1.5/rfmanalysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      524 2023-05-16 22:17:58.000000 rfmanalysis-0.1.5/rfmanalysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 22:17:58.000000 rfmanalysis-0.1.5/rfmanalysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-16 18:47:20.000000 rfmanalysis-0.1.5/rfmanalysis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-05-16 22:17:58.000000 rfmanalysis-0.1.5/rfmanalysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      454 2023-05-16 22:17:59.008002 rfmanalysis-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1658 2023-05-16 22:17:27.000000 rfmanalysis-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:17:58.994896 rfmanalysis-0.1.5/tests/
+-rw-rw-rw-   0        0        0       42 2023-05-16 18:36:44.000000 rfmanalysis-0.1.5/tests/__init__.py
+-rw-rw-rw-   0        0        0      589 2023-05-16 18:36:44.000000 rfmanalysis-0.1.5/tests/test_rfmanalysis.py
```

### Comparing `rfmanalysis-0.1.4/CONTRIBUTING.rst` & `rfmanalysis-0.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.4/LICENSE` & `rfmanalysis-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.4/PKG-INFO` & `rfmanalysis-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfmanalysis
-Version: 0.1.4
+Version: 0.1.5
 Summary: This repository contains a Python implementation of RFM (Recency, Frequency, Monetary) analysis, a customer segmentation technique used in marketing and customer relationship management. The RFM analysis helps identify customer segments based on their purchasing behavior, allowing businesses to tailor their marketing strategies and customer retention efforts.
 Home-page: https://github.com/emmayann/rfmanalysis
 Author: Emma Hovhannisyan
 Author-email: emmahovhannisyan02@gmail.com
 License: MIT license
 Keywords: rfmanalysis
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `rfmanalysis-0.1.4/README.rst` & `rfmanalysis-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.4/docs/Makefile` & `rfmanalysis-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.4/docs/conf.py` & `rfmanalysis-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.4/docs/installation.rst` & `rfmanalysis-0.1.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.4/docs/make.bat` & `rfmanalysis-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.4/rfmanalysis/rfmanalysis.py` & `rfmanalysis-0.1.5/rfmanalysis/rfmanalysis.py`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.4/rfmanalysis.egg-info/PKG-INFO` & `rfmanalysis-0.1.5/rfmanalysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfmanalysis
-Version: 0.1.4
+Version: 0.1.5
 Summary: This repository contains a Python implementation of RFM (Recency, Frequency, Monetary) analysis, a customer segmentation technique used in marketing and customer relationship management. The RFM analysis helps identify customer segments based on their purchasing behavior, allowing businesses to tailor their marketing strategies and customer retention efforts.
 Home-page: https://github.com/emmayann/rfmanalysis
 Author: Emma Hovhannisyan
 Author-email: emmahovhannisyan02@gmail.com
 License: MIT license
 Keywords: rfmanalysis
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `rfmanalysis-0.1.4/rfmanalysis.egg-info/SOURCES.txt` & `rfmanalysis-0.1.5/rfmanalysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.4/setup.py` & `rfmanalysis-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords='rfmanalysis',
     name='rfmanalysis',
     packages=find_packages(include=['rfmanalysis', 'rfmanalysis.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/emmayann/rfmanalysis',
-    version='0.1.4',
+    version='0.1.5',
     zip_safe=False,
 )
```

### Comparing `rfmanalysis-0.1.4/tests/test_rfmanalysis.py` & `rfmanalysis-0.1.5/tests/test_rfmanalysis.py`

 * *Files identical despite different names*

