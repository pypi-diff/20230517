# Comparing `tmp/payok.io-1.0.1.tar.gz` & `tmp/payok.io-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payok.io-1.0.1.tar", last modified: Wed May 17 15:01:41 2023, max compression
+gzip compressed data, was "payok.io-1.0.2.tar", last modified: Wed May 17 15:10:43 2023, max compression
```

## Comparing `payok.io-1.0.1.tar` & `payok.io-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-17 15:01:41.818463 payok.io-1.0.1/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     1063 2023-05-17 13:59:37.000000 payok.io-1.0.1/LICENSE
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     2303 2023-05-17 15:01:41.818463 payok.io-1.0.1/PKG-INFO
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     1512 2023-05-17 13:45:53.000000 payok.io-1.0.1/README.md
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-17 15:01:41.814463 payok.io-1.0.1/payok/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      494 2023-05-17 14:50:33.000000 payok.io-1.0.1/payok/__init__.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     7300 2023-05-17 15:01:27.000000 payok.io-1.0.1/payok/api.py
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-17 15:01:41.818463 payok.io-1.0.1/payok/enums/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      362 2023-05-17 13:37:52.000000 payok.io-1.0.1/payok/enums/__init__.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      162 2023-05-17 14:34:42.000000 payok.io-1.0.1/payok/enums/base.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      114 2023-05-17 14:34:58.000000 payok.io-1.0.1/payok/enums/comission_type.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      138 2023-05-17 14:35:37.000000 payok.io-1.0.1/payok/enums/currency.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)       99 2023-05-17 14:38:46.000000 payok.io-1.0.1/payok/enums/pay_status.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      293 2023-05-17 14:35:18.000000 payok.io-1.0.1/payok/enums/payment_method.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      455 2023-05-17 14:35:26.000000 payok.io-1.0.1/payok/enums/payout_method.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      103 2023-05-17 14:20:25.000000 payok.io-1.0.1/payok/enums/webhook_status.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      272 2023-05-17 14:06:53.000000 payok.io-1.0.1/payok/exceptions.py
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-17 15:01:41.818463 payok.io-1.0.1/payok/models/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      208 2023-05-17 14:49:34.000000 payok.io-1.0.1/payok/models/__init__.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      139 2023-05-16 21:14:21.000000 payok.io-1.0.1/payok/models/balance.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      196 2023-05-17 14:49:19.000000 payok.io-1.0.1/payok/models/new_payout.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      898 2023-05-17 14:55:52.000000 payok.io-1.0.1/payok/models/payout.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      967 2023-05-17 14:25:29.000000 payok.io-1.0.1/payok/models/transaction.py
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-17 15:01:41.818463 payok.io-1.0.1/payok.io.egg-info/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     2303 2023-05-17 15:01:41.000000 payok.io-1.0.1/payok.io.egg-info/PKG-INFO
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      576 2023-05-17 15:01:41.000000 payok.io-1.0.1/payok.io.egg-info/SOURCES.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)        1 2023-05-17 15:01:41.000000 payok.io-1.0.1/payok.io.egg-info/dependency_links.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)       17 2023-05-17 15:01:41.000000 payok.io-1.0.1/payok.io.egg-info/requires.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)        6 2023-05-17 15:01:41.000000 payok.io-1.0.1/payok.io.egg-info/top_level.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)       38 2023-05-17 15:01:41.818463 payok.io-1.0.1/setup.cfg
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     1269 2023-05-17 15:01:14.000000 payok.io-1.0.1/setup.py
+drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-17 15:10:43.908498 payok.io-1.0.2/
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     1063 2023-05-17 13:59:37.000000 payok.io-1.0.2/LICENSE
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     2309 2023-05-17 15:10:43.908498 payok.io-1.0.2/PKG-INFO
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     1518 2023-05-17 15:09:15.000000 payok.io-1.0.2/README.md
+drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-17 15:10:43.904498 payok.io-1.0.2/payok/
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      494 2023-05-17 14:50:33.000000 payok.io-1.0.2/payok/__init__.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     7300 2023-05-17 15:01:27.000000 payok.io-1.0.2/payok/api.py
+drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-17 15:10:43.904498 payok.io-1.0.2/payok/enums/
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      362 2023-05-17 13:37:52.000000 payok.io-1.0.2/payok/enums/__init__.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      162 2023-05-17 14:34:42.000000 payok.io-1.0.2/payok/enums/base.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      114 2023-05-17 14:34:58.000000 payok.io-1.0.2/payok/enums/comission_type.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      138 2023-05-17 14:35:37.000000 payok.io-1.0.2/payok/enums/currency.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)       99 2023-05-17 14:38:46.000000 payok.io-1.0.2/payok/enums/pay_status.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      293 2023-05-17 14:35:18.000000 payok.io-1.0.2/payok/enums/payment_method.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      455 2023-05-17 14:35:26.000000 payok.io-1.0.2/payok/enums/payout_method.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      103 2023-05-17 14:20:25.000000 payok.io-1.0.2/payok/enums/webhook_status.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      272 2023-05-17 14:06:53.000000 payok.io-1.0.2/payok/exceptions.py
+drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-17 15:10:43.908498 payok.io-1.0.2/payok/models/
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      208 2023-05-17 14:49:34.000000 payok.io-1.0.2/payok/models/__init__.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      139 2023-05-16 21:14:21.000000 payok.io-1.0.2/payok/models/balance.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      196 2023-05-17 14:49:19.000000 payok.io-1.0.2/payok/models/new_payout.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      898 2023-05-17 14:55:52.000000 payok.io-1.0.2/payok/models/payout.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      967 2023-05-17 14:25:29.000000 payok.io-1.0.2/payok/models/transaction.py
+drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-17 15:10:43.904498 payok.io-1.0.2/payok.io.egg-info/
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     2309 2023-05-17 15:10:43.000000 payok.io-1.0.2/payok.io.egg-info/PKG-INFO
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      576 2023-05-17 15:10:43.000000 payok.io-1.0.2/payok.io.egg-info/SOURCES.txt
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)        1 2023-05-17 15:10:43.000000 payok.io-1.0.2/payok.io.egg-info/dependency_links.txt
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)       17 2023-05-17 15:10:43.000000 payok.io-1.0.2/payok.io.egg-info/requires.txt
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)        6 2023-05-17 15:10:43.000000 payok.io-1.0.2/payok.io.egg-info/top_level.txt
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)       38 2023-05-17 15:10:43.908498 payok.io-1.0.2/setup.cfg
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     1269 2023-05-17 15:10:05.000000 payok.io-1.0.2/setup.py
```

### Comparing `payok.io-1.0.1/LICENSE` & `payok.io-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `payok.io-1.0.1/PKG-INFO` & `payok.io-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payok.io
-Version: 1.0.1
+Version: 1.0.2
 Summary: Asynchronous PayOK API wrapper
 Home-page: https://github.com/nikitalm8/payok
 Author: Nikita Minaev
 Author-email: <nikita@minaev.su>
 Project-URL: Homepage, https://github.com/nikitalm8/payok
 Project-URL: Bug Tracker, https://github.com/nikitalm8/payok/issues
 Project-URL: API Docs, https://payok.io/cabinet/documentation/doc_api_main
@@ -18,24 +18,24 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <div align="left">
     <h1>PayOK    <img src="https://payok.io/files/image/logo_white.svg" width=64 height=24></h1>
     <p align="left" >
-        <a href="https://pypi.org/project/payok/">
+        <a href="https://pypi.org/project/payok.io/">
             <img src="https://img.shields.io/pypi/v/payok.io?style=flat-square" alt="PyPI">
         </a>
-        <a href="https://pypi.org/project/payok/">
+        <a href="https://pypi.org/project/payok.io/">
             <img src="https://img.shields.io/pypi/dm/payok.io?style=flat-square" alt="PyPI">
         </a>
     </p>
 </div>
 
-A simple, yet powerful library for PayOK [API](https://payok.io/cabinet/documentation/doc_api_main)
+A simple, yet powerful library for [PayOK API](https://payok.io/cabinet/documentation/doc_api_main)
 
 
 ## Usage
 
 With ``PayOK`` you can easily create and retrieve payment and payout info, get informaition about your account's balance and commissions, etc.
 
 ## Documentation
```

### Comparing `payok.io-1.0.1/README.md` & `payok.io-1.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 <div align="left">
     <h1>PayOK    <img src="https://payok.io/files/image/logo_white.svg" width=64 height=24></h1>
     <p align="left" >
-        <a href="https://pypi.org/project/payok/">
+        <a href="https://pypi.org/project/payok.io/">
             <img src="https://img.shields.io/pypi/v/payok.io?style=flat-square" alt="PyPI">
         </a>
-        <a href="https://pypi.org/project/payok/">
+        <a href="https://pypi.org/project/payok.io/">
             <img src="https://img.shields.io/pypi/dm/payok.io?style=flat-square" alt="PyPI">
         </a>
     </p>
 </div>
 
-A simple, yet powerful library for PayOK [API](https://payok.io/cabinet/documentation/doc_api_main)
+A simple, yet powerful library for [PayOK API](https://payok.io/cabinet/documentation/doc_api_main)
 
 
 ## Usage
 
 With ``PayOK`` you can easily create and retrieve payment and payout info, get informaition about your account's balance and commissions, etc.
 
 ## Documentation
```

### Comparing `payok.io-1.0.1/payok/api.py` & `payok.io-1.0.2/payok/api.py`

 * *Files identical despite different names*

### Comparing `payok.io-1.0.1/payok/models/payout.py` & `payok.io-1.0.2/payok/models/payout.py`

 * *Files identical despite different names*

### Comparing `payok.io-1.0.1/payok/models/transaction.py` & `payok.io-1.0.2/payok/models/transaction.py`

 * *Files identical despite different names*

### Comparing `payok.io-1.0.1/payok.io.egg-info/PKG-INFO` & `payok.io-1.0.2/payok.io.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payok.io
-Version: 1.0.1
+Version: 1.0.2
 Summary: Asynchronous PayOK API wrapper
 Home-page: https://github.com/nikitalm8/payok
 Author: Nikita Minaev
 Author-email: <nikita@minaev.su>
 Project-URL: Homepage, https://github.com/nikitalm8/payok
 Project-URL: Bug Tracker, https://github.com/nikitalm8/payok/issues
 Project-URL: API Docs, https://payok.io/cabinet/documentation/doc_api_main
@@ -18,24 +18,24 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <div align="left">
     <h1>PayOK    <img src="https://payok.io/files/image/logo_white.svg" width=64 height=24></h1>
     <p align="left" >
-        <a href="https://pypi.org/project/payok/">
+        <a href="https://pypi.org/project/payok.io/">
             <img src="https://img.shields.io/pypi/v/payok.io?style=flat-square" alt="PyPI">
         </a>
-        <a href="https://pypi.org/project/payok/">
+        <a href="https://pypi.org/project/payok.io/">
             <img src="https://img.shields.io/pypi/dm/payok.io?style=flat-square" alt="PyPI">
         </a>
     </p>
 </div>
 
-A simple, yet powerful library for PayOK [API](https://payok.io/cabinet/documentation/doc_api_main)
+A simple, yet powerful library for [PayOK API](https://payok.io/cabinet/documentation/doc_api_main)
 
 
 ## Usage
 
 With ``PayOK`` you can easily create and retrieve payment and payout info, get informaition about your account's balance and commissions, etc.
 
 ## Documentation
```

### Comparing `payok.io-1.0.1/payok.io.egg-info/SOURCES.txt` & `payok.io-1.0.2/payok.io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `payok.io-1.0.1/setup.py` & `payok.io-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as file:
 
     long_description = "\n" + file.read()
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'Asynchronous PayOK API wrapper'
 
 setup(
     name="payok.io",
     version=VERSION,
     author="Nikita Minaev",
     author_email="<nikita@minaev.su>",
```

