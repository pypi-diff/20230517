# Comparing `tmp/sisU_gmail_loren-magnuson-0.0.3rc0.tar.gz` & `tmp/sisu_gmail_loren-magnuson-0.0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sisU_gmail_loren-magnuson-0.0.3rc0.tar", last modified: Wed May 17 21:45:21 2023, max compression
+gzip compressed data, was "sisu_gmail_loren-magnuson-0.0.4a0.tar", last modified: Wed May 17 21:48:18 2023, max compression
```

## Comparing `sisU_gmail_loren-magnuson-0.0.3rc0.tar` & `sisu_gmail_loren-magnuson-0.0.4a0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 loren     (1000) loren     (1000)        0 2023-05-17 21:45:21.013667 sisU_gmail_loren-magnuson-0.0.3rc0/
--rw-rw-r--   0 loren     (1000) loren     (1000)    35147 2023-05-17 18:27:11.000000 sisU_gmail_loren-magnuson-0.0.3rc0/LICENSE
--rw-rw-r--   0 loren     (1000) loren     (1000)     1122 2023-05-17 21:45:21.013667 sisU_gmail_loren-magnuson-0.0.3rc0/PKG-INFO
--rw-rw-r--   0 loren     (1000) loren     (1000)      573 2023-05-17 18:27:11.000000 sisU_gmail_loren-magnuson-0.0.3rc0/README.md
--rw-rw-r--   0 loren     (1000) loren     (1000)      103 2023-05-17 18:27:11.000000 sisU_gmail_loren-magnuson-0.0.3rc0/pyproject.toml
--rw-rw-r--   0 loren     (1000) loren     (1000)      672 2023-05-17 21:45:21.013667 sisU_gmail_loren-magnuson-0.0.3rc0/setup.cfg
-drwxrwxr-x   0 loren     (1000) loren     (1000)        0 2023-05-17 21:45:21.009667 sisU_gmail_loren-magnuson-0.0.3rc0/src/
-drwxrwxr-x   0 loren     (1000) loren     (1000)        0 2023-05-17 21:45:21.009667 sisU_gmail_loren-magnuson-0.0.3rc0/src/sisU_gmail_loren_magnuson.egg-info/
--rw-rw-r--   0 loren     (1000) loren     (1000)     1122 2023-05-17 21:45:21.000000 sisU_gmail_loren-magnuson-0.0.3rc0/src/sisU_gmail_loren_magnuson.egg-info/PKG-INFO
--rw-rw-r--   0 loren     (1000) loren     (1000)      631 2023-05-17 21:45:21.000000 sisU_gmail_loren-magnuson-0.0.3rc0/src/sisU_gmail_loren_magnuson.egg-info/SOURCES.txt
--rw-rw-r--   0 loren     (1000) loren     (1000)        1 2023-05-17 21:45:21.000000 sisU_gmail_loren-magnuson-0.0.3rc0/src/sisU_gmail_loren_magnuson.egg-info/dependency_links.txt
--rw-rw-r--   0 loren     (1000) loren     (1000)       11 2023-05-17 21:45:21.000000 sisU_gmail_loren-magnuson-0.0.3rc0/src/sisU_gmail_loren_magnuson.egg-info/top_level.txt
-drwxrwxr-x   0 loren     (1000) loren     (1000)        0 2023-05-17 21:45:21.013667 sisU_gmail_loren-magnuson-0.0.3rc0/src/sisu_gmail/
--rw-rw-r--   0 loren     (1000) loren     (1000)      159 2023-05-17 18:27:11.000000 sisU_gmail_loren-magnuson-0.0.3rc0/src/sisu_gmail/__init__.py
--rw-rw-r--   0 loren     (1000) loren     (1000)     1975 2023-05-17 18:27:11.000000 sisU_gmail_loren-magnuson-0.0.3rc0/src/sisu_gmail/auth.py
--rw-rw-r--   0 loren     (1000) loren     (1000)      330 2023-05-17 18:39:58.000000 sisU_gmail_loren-magnuson-0.0.3rc0/src/sisu_gmail/create.py
--rw-rw-r--   0 loren     (1000) loren     (1000)      892 2023-05-17 18:27:11.000000 sisU_gmail_loren-magnuson-0.0.3rc0/src/sisu_gmail/delete.py
--rw-rw-r--   0 loren     (1000) loren     (1000)     2088 2023-05-17 18:27:11.000000 sisU_gmail_loren-magnuson-0.0.3rc0/src/sisu_gmail/label.py
--rw-rw-r--   0 loren     (1000) loren     (1000)      377 2023-05-17 18:27:11.000000 sisU_gmail_loren-magnuson-0.0.3rc0/src/sisu_gmail/read.py
--rw-rw-r--   0 loren     (1000) loren     (1000)     2405 2023-05-17 21:35:03.000000 sisU_gmail_loren-magnuson-0.0.3rc0/src/sisu_gmail/search.py
--rw-rw-r--   0 loren     (1000) loren     (1000)      387 2023-05-17 18:27:11.000000 sisU_gmail_loren-magnuson-0.0.3rc0/src/sisu_gmail/send.py
--rw-rw-r--   0 loren     (1000) loren     (1000)      295 2023-05-17 18:27:11.000000 sisU_gmail_loren-magnuson-0.0.3rc0/src/sisu_gmail/user.py
-drwxrwxr-x   0 loren     (1000) loren     (1000)        0 2023-05-17 21:45:21.013667 sisU_gmail_loren-magnuson-0.0.3rc0/tests/
--rw-rw-r--   0 loren     (1000) loren     (1000)     1489 2023-05-17 18:27:11.000000 sisU_gmail_loren-magnuson-0.0.3rc0/tests/test_auth.py
--rw-rw-r--   0 loren     (1000) loren     (1000)      917 2023-05-17 18:27:11.000000 sisU_gmail_loren-magnuson-0.0.3rc0/tests/test_create.py
--rw-rw-r--   0 loren     (1000) loren     (1000)     2109 2023-05-17 18:27:11.000000 sisU_gmail_loren-magnuson-0.0.3rc0/tests/test_delete.py
--rw-rw-r--   0 loren     (1000) loren     (1000)     4416 2023-05-17 18:27:11.000000 sisU_gmail_loren-magnuson-0.0.3rc0/tests/test_label.py
--rw-rw-r--   0 loren     (1000) loren     (1000)      713 2023-05-17 18:27:11.000000 sisU_gmail_loren-magnuson-0.0.3rc0/tests/test_read.py
--rw-rw-r--   0 loren     (1000) loren     (1000)     2382 2023-05-17 21:36:11.000000 sisU_gmail_loren-magnuson-0.0.3rc0/tests/test_search.py
--rw-rw-r--   0 loren     (1000) loren     (1000)     1336 2023-05-17 18:27:11.000000 sisU_gmail_loren-magnuson-0.0.3rc0/tests/test_send.py
--rw-rw-r--   0 loren     (1000) loren     (1000)      444 2023-05-17 18:27:11.000000 sisU_gmail_loren-magnuson-0.0.3rc0/tests/test_user.py
+drwxrwxr-x   0 loren     (1000) loren     (1000)        0 2023-05-17 21:48:17.998381 sisu_gmail_loren-magnuson-0.0.4a0/
+-rw-rw-r--   0 loren     (1000) loren     (1000)    35147 2023-05-17 18:27:11.000000 sisu_gmail_loren-magnuson-0.0.4a0/LICENSE
+-rw-rw-r--   0 loren     (1000) loren     (1000)     1121 2023-05-17 21:48:17.998381 sisu_gmail_loren-magnuson-0.0.4a0/PKG-INFO
+-rw-rw-r--   0 loren     (1000) loren     (1000)      573 2023-05-17 18:27:11.000000 sisu_gmail_loren-magnuson-0.0.4a0/README.md
+-rw-rw-r--   0 loren     (1000) loren     (1000)      103 2023-05-17 18:27:11.000000 sisu_gmail_loren-magnuson-0.0.4a0/pyproject.toml
+-rw-rw-r--   0 loren     (1000) loren     (1000)      672 2023-05-17 21:48:17.998381 sisu_gmail_loren-magnuson-0.0.4a0/setup.cfg
+drwxrwxr-x   0 loren     (1000) loren     (1000)        0 2023-05-17 21:48:17.994382 sisu_gmail_loren-magnuson-0.0.4a0/src/
+drwxrwxr-x   0 loren     (1000) loren     (1000)        0 2023-05-17 21:48:17.994382 sisu_gmail_loren-magnuson-0.0.4a0/src/sisu_gmail/
+-rw-rw-r--   0 loren     (1000) loren     (1000)      159 2023-05-17 18:27:11.000000 sisu_gmail_loren-magnuson-0.0.4a0/src/sisu_gmail/__init__.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)     1975 2023-05-17 18:27:11.000000 sisu_gmail_loren-magnuson-0.0.4a0/src/sisu_gmail/auth.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)      330 2023-05-17 18:39:58.000000 sisu_gmail_loren-magnuson-0.0.4a0/src/sisu_gmail/create.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)      892 2023-05-17 18:27:11.000000 sisu_gmail_loren-magnuson-0.0.4a0/src/sisu_gmail/delete.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)     2088 2023-05-17 18:27:11.000000 sisu_gmail_loren-magnuson-0.0.4a0/src/sisu_gmail/label.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)      377 2023-05-17 18:27:11.000000 sisu_gmail_loren-magnuson-0.0.4a0/src/sisu_gmail/read.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)     2405 2023-05-17 21:35:03.000000 sisu_gmail_loren-magnuson-0.0.4a0/src/sisu_gmail/search.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)      387 2023-05-17 18:27:11.000000 sisu_gmail_loren-magnuson-0.0.4a0/src/sisu_gmail/send.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)      295 2023-05-17 18:27:11.000000 sisu_gmail_loren-magnuson-0.0.4a0/src/sisu_gmail/user.py
+drwxrwxr-x   0 loren     (1000) loren     (1000)        0 2023-05-17 21:48:17.998381 sisu_gmail_loren-magnuson-0.0.4a0/src/sisu_gmail_loren_magnuson.egg-info/
+-rw-rw-r--   0 loren     (1000) loren     (1000)     1121 2023-05-17 21:48:17.000000 sisu_gmail_loren-magnuson-0.0.4a0/src/sisu_gmail_loren_magnuson.egg-info/PKG-INFO
+-rw-rw-r--   0 loren     (1000) loren     (1000)      631 2023-05-17 21:48:17.000000 sisu_gmail_loren-magnuson-0.0.4a0/src/sisu_gmail_loren_magnuson.egg-info/SOURCES.txt
+-rw-rw-r--   0 loren     (1000) loren     (1000)        1 2023-05-17 21:48:17.000000 sisu_gmail_loren-magnuson-0.0.4a0/src/sisu_gmail_loren_magnuson.egg-info/dependency_links.txt
+-rw-rw-r--   0 loren     (1000) loren     (1000)       11 2023-05-17 21:48:17.000000 sisu_gmail_loren-magnuson-0.0.4a0/src/sisu_gmail_loren_magnuson.egg-info/top_level.txt
+drwxrwxr-x   0 loren     (1000) loren     (1000)        0 2023-05-17 21:48:17.998381 sisu_gmail_loren-magnuson-0.0.4a0/tests/
+-rw-rw-r--   0 loren     (1000) loren     (1000)     1489 2023-05-17 18:27:11.000000 sisu_gmail_loren-magnuson-0.0.4a0/tests/test_auth.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)      917 2023-05-17 18:27:11.000000 sisu_gmail_loren-magnuson-0.0.4a0/tests/test_create.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)     2109 2023-05-17 18:27:11.000000 sisu_gmail_loren-magnuson-0.0.4a0/tests/test_delete.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)     4416 2023-05-17 18:27:11.000000 sisu_gmail_loren-magnuson-0.0.4a0/tests/test_label.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)      713 2023-05-17 18:27:11.000000 sisu_gmail_loren-magnuson-0.0.4a0/tests/test_read.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)     2382 2023-05-17 21:36:11.000000 sisu_gmail_loren-magnuson-0.0.4a0/tests/test_search.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)     1336 2023-05-17 18:27:11.000000 sisu_gmail_loren-magnuson-0.0.4a0/tests/test_send.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)      444 2023-05-17 18:27:11.000000 sisu_gmail_loren-magnuson-0.0.4a0/tests/test_user.py
```

### Comparing `sisU_gmail_loren-magnuson-0.0.3rc0/LICENSE` & `sisu_gmail_loren-magnuson-0.0.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `sisU_gmail_loren-magnuson-0.0.3rc0/PKG-INFO` & `sisu_gmail_loren-magnuson-0.0.4a0/src/sisu_gmail_loren_magnuson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sisU_gmail_loren-magnuson
-Version: 0.0.3rc0
+Name: sisu-gmail-loren-magnuson
+Version: 0.0.4a0
 Summary: A package to simplify my gmail api life
 Home-page: https://github.com/loren-magnuson/sisu_gmail
 Author: Loren Magnuson
 Author-email: lorenjmagnuson@gmail.com
 Project-URL: Bug Tracker, https://github.com/loren-magnuson/sisu_gmail/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sisU_gmail_loren-magnuson-0.0.3rc0/README.md` & `sisu_gmail_loren-magnuson-0.0.4a0/README.md`

 * *Files identical despite different names*

### Comparing `sisU_gmail_loren-magnuson-0.0.3rc0/setup.cfg` & `sisu_gmail_loren-magnuson-0.0.4a0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
-name = sisU_gmail_loren-magnuson
-version = 0.0.3c
+name = sisu_gmail_loren-magnuson
+version = 0.0.4a
 author = Loren Magnuson
 author_email = lorenjmagnuson@gmail.com
 description = A package to simplify my gmail api life
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/loren-magnuson/sisu_gmail
 project_urls =
```

### Comparing `sisU_gmail_loren-magnuson-0.0.3rc0/src/sisU_gmail_loren_magnuson.egg-info/PKG-INFO` & `sisu_gmail_loren-magnuson-0.0.4a0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sisU-gmail-loren-magnuson
-Version: 0.0.3rc0
+Name: sisu_gmail_loren-magnuson
+Version: 0.0.4a0
 Summary: A package to simplify my gmail api life
 Home-page: https://github.com/loren-magnuson/sisu_gmail
 Author: Loren Magnuson
 Author-email: lorenjmagnuson@gmail.com
 Project-URL: Bug Tracker, https://github.com/loren-magnuson/sisu_gmail/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sisU_gmail_loren-magnuson-0.0.3rc0/src/sisu_gmail/auth.py` & `sisu_gmail_loren-magnuson-0.0.4a0/src/sisu_gmail/auth.py`

 * *Files identical despite different names*

### Comparing `sisU_gmail_loren-magnuson-0.0.3rc0/src/sisu_gmail/delete.py` & `sisu_gmail_loren-magnuson-0.0.4a0/src/sisu_gmail/delete.py`

 * *Files identical despite different names*

### Comparing `sisU_gmail_loren-magnuson-0.0.3rc0/src/sisu_gmail/label.py` & `sisu_gmail_loren-magnuson-0.0.4a0/src/sisu_gmail/label.py`

 * *Files identical despite different names*

### Comparing `sisU_gmail_loren-magnuson-0.0.3rc0/src/sisu_gmail/search.py` & `sisu_gmail_loren-magnuson-0.0.4a0/src/sisu_gmail/search.py`

 * *Files identical despite different names*

### Comparing `sisU_gmail_loren-magnuson-0.0.3rc0/tests/test_auth.py` & `sisu_gmail_loren-magnuson-0.0.4a0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `sisU_gmail_loren-magnuson-0.0.3rc0/tests/test_create.py` & `sisu_gmail_loren-magnuson-0.0.4a0/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `sisU_gmail_loren-magnuson-0.0.3rc0/tests/test_delete.py` & `sisu_gmail_loren-magnuson-0.0.4a0/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `sisU_gmail_loren-magnuson-0.0.3rc0/tests/test_label.py` & `sisu_gmail_loren-magnuson-0.0.4a0/tests/test_label.py`

 * *Files identical despite different names*

### Comparing `sisU_gmail_loren-magnuson-0.0.3rc0/tests/test_read.py` & `sisu_gmail_loren-magnuson-0.0.4a0/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `sisU_gmail_loren-magnuson-0.0.3rc0/tests/test_search.py` & `sisu_gmail_loren-magnuson-0.0.4a0/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `sisU_gmail_loren-magnuson-0.0.3rc0/tests/test_send.py` & `sisu_gmail_loren-magnuson-0.0.4a0/tests/test_send.py`

 * *Files identical despite different names*

