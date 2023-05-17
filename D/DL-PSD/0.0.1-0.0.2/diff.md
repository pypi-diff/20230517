# Comparing `tmp/DL_PSD-0.0.1.tar.gz` & `tmp/DL_PSD-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DL_PSD-0.0.1.tar", last modified: Wed May 17 07:02:38 2023, max compression
+gzip compressed data, was "DL_PSD-0.0.2.tar", last modified: Wed May 17 07:08:15 2023, max compression
```

## Comparing `DL_PSD-0.0.1.tar` & `DL_PSD-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 07:02:38.765501 DL_PSD-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-17 07:02:38.703005 DL_PSD-0.0.1/DL_PSD/
--rw-rw-rw-   0        0        0    11253 2023-05-17 06:46:49.000000 DL_PSD-0.0.1/DL_PSD/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 07:02:38.749876 DL_PSD-0.0.1/DL_PSD.egg-info/
--rw-rw-rw-   0        0        0      550 2023-05-17 07:02:38.000000 DL_PSD-0.0.1/DL_PSD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-05-17 07:02:38.000000 DL_PSD-0.0.1/DL_PSD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 07:02:38.000000 DL_PSD-0.0.1/DL_PSD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-17 07:02:38.000000 DL_PSD-0.0.1/DL_PSD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1057 2023-05-17 06:46:46.000000 DL_PSD-0.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0       24 2023-05-17 06:46:44.000000 DL_PSD-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      550 2023-05-17 07:02:38.749876 DL_PSD-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-05-17 06:46:43.000000 DL_PSD-0.0.1/README.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 07:02:38.765501 DL_PSD-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      620 2023-05-17 07:02:22.000000 DL_PSD-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:08:15.454165 DL_PSD-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-17 07:08:15.376046 DL_PSD-0.0.2/DL_PSD/
+-rw-rw-rw-   0        0        0    11253 2023-05-17 06:46:49.000000 DL_PSD-0.0.2/DL_PSD/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:08:15.422919 DL_PSD-0.0.2/DL_PSD.egg-info/
+-rw-rw-rw-   0        0        0      608 2023-05-17 07:08:15.000000 DL_PSD-0.0.2/DL_PSD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-05-17 07:08:15.000000 DL_PSD-0.0.2/DL_PSD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 07:08:15.000000 DL_PSD-0.0.2/DL_PSD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-17 07:08:15.000000 DL_PSD-0.0.2/DL_PSD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-17 07:08:15.000000 DL_PSD-0.0.2/DL_PSD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1057 2023-05-17 06:46:46.000000 DL_PSD-0.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       24 2023-05-17 06:46:44.000000 DL_PSD-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      608 2023-05-17 07:08:15.438542 DL_PSD-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-05-17 06:46:43.000000 DL_PSD-0.0.2/README.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 07:08:15.454165 DL_PSD-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      973 2023-05-17 07:08:08.000000 DL_PSD-0.0.2/setup.py
```

### Comparing `DL_PSD-0.0.1/DL_PSD/__init__.py` & `DL_PSD-0.0.2/DL_PSD/__init__.py`

 * *Files identical despite different names*

### Comparing `DL_PSD-0.0.1/LICENCE.txt` & `DL_PSD-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `DL_PSD-0.0.1/PKG-INFO` & `DL_PSD-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: DL_PSD
-Version: 0.0.1
+Version: 0.0.2
 Summary: PSD calc
-Home-page: 
-Author: B
-Author-email: 
+Home-page: https://github.com/username/repo
+Author: Brinthan
+Author-email: kbrinthan.22@uom.lk
 License: MIT
 Keywords: calculator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

