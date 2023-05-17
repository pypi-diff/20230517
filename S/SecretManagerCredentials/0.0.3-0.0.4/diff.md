# Comparing `tmp/SecretManagerCredentials-0.0.3.tar.gz` & `tmp/SecretManagerCredentials-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SecretManagerCredentials-0.0.3.tar", last modified: Tue May 16 21:18:23 2023, max compression
+gzip compressed data, was "SecretManagerCredentials-0.0.4.tar", last modified: Tue May 16 22:02:25 2023, max compression
```

## Comparing `SecretManagerCredentials-0.0.3.tar` & `SecretManagerCredentials-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 21:18:23.011822 SecretManagerCredentials-0.0.3/
--rw-rw-rw-   0        0        0     1094 2023-05-08 06:01:05.000000 SecretManagerCredentials-0.0.3/Licence
--rw-rw-rw-   0        0        0     2151 2023-05-16 21:18:23.012823 SecretManagerCredentials-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1524 2023-05-08 06:01:05.000000 SecretManagerCredentials-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 21:18:22.991937 SecretManagerCredentials-0.0.3/SecretManagerCredentials/
--rw-rw-rw-   0        0        0    10199 2023-05-16 21:17:33.000000 SecretManagerCredentials-0.0.3/SecretManagerCredentials/SecretManagerFetcher.py
--rw-rw-rw-   0        0        0      143 2023-05-16 21:17:42.000000 SecretManagerCredentials-0.0.3/SecretManagerCredentials/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:18:23.008819 SecretManagerCredentials-0.0.3/SecretManagerCredentials.egg-info/
--rw-rw-rw-   0        0        0     2151 2023-05-16 21:18:22.000000 SecretManagerCredentials-0.0.3/SecretManagerCredentials.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-05-16 21:18:22.000000 SecretManagerCredentials-0.0.3/SecretManagerCredentials.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 21:18:22.000000 SecretManagerCredentials-0.0.3/SecretManagerCredentials.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-16 21:18:22.000000 SecretManagerCredentials-0.0.3/SecretManagerCredentials.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-05-16 21:18:22.000000 SecretManagerCredentials-0.0.3/SecretManagerCredentials.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       83 2023-05-16 21:18:23.014820 SecretManagerCredentials-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1652 2023-05-16 12:39:53.000000 SecretManagerCredentials-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:02:25.000558 SecretManagerCredentials-0.0.4/
+-rw-rw-rw-   0        0        0     1094 2023-05-08 06:01:05.000000 SecretManagerCredentials-0.0.4/Licence
+-rw-rw-rw-   0        0        0     2151 2023-05-16 22:02:25.001665 SecretManagerCredentials-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1524 2023-05-08 06:01:05.000000 SecretManagerCredentials-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 22:02:24.979913 SecretManagerCredentials-0.0.4/SecretManagerCredentials/
+-rw-rw-rw-   0        0        0    10199 2023-05-16 21:17:33.000000 SecretManagerCredentials-0.0.4/SecretManagerCredentials/SecretManagerFetcher.py
+-rw-rw-rw-   0        0        0      143 2023-05-16 22:01:36.000000 SecretManagerCredentials-0.0.4/SecretManagerCredentials/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:02:24.997575 SecretManagerCredentials-0.0.4/SecretManagerCredentials.egg-info/
+-rw-rw-rw-   0        0        0     2151 2023-05-16 22:02:24.000000 SecretManagerCredentials-0.0.4/SecretManagerCredentials.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-05-16 22:02:24.000000 SecretManagerCredentials-0.0.4/SecretManagerCredentials.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 22:02:24.000000 SecretManagerCredentials-0.0.4/SecretManagerCredentials.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-16 22:02:24.000000 SecretManagerCredentials-0.0.4/SecretManagerCredentials.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-05-16 22:02:24.000000 SecretManagerCredentials-0.0.4/SecretManagerCredentials.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       83 2023-05-16 22:02:25.004644 SecretManagerCredentials-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1652 2023-05-16 12:39:53.000000 SecretManagerCredentials-0.0.4/setup.py
```

### Comparing `SecretManagerCredentials-0.0.3/Licence` & `SecretManagerCredentials-0.0.4/Licence`

 * *Files identical despite different names*

### Comparing `SecretManagerCredentials-0.0.3/PKG-INFO` & `SecretManagerCredentials-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecretManagerCredentials
-Version: 0.0.3
+Version: 0.0.4
 Summary: Convenient wrapper for executing codes on AWS for connecting and fetching credentials from vault
 Home-page: 
 Download-URL: 
 Author: Mallikarjuna Devaraya
 License: MIT
 Keywords: Vault Credential Fetch,Credential Fetch,Vault
 Classifier: Development Status :: 4 - Beta
```

### Comparing `SecretManagerCredentials-0.0.3/README.md` & `SecretManagerCredentials-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `SecretManagerCredentials-0.0.3/SecretManagerCredentials/SecretManagerFetcher.py` & `SecretManagerCredentials-0.0.4/SecretManagerCredentials/SecretManagerFetcher.py`

 * *Files identical despite different names*

### Comparing `SecretManagerCredentials-0.0.3/SecretManagerCredentials.egg-info/PKG-INFO` & `SecretManagerCredentials-0.0.4/SecretManagerCredentials.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecretManagerCredentials
-Version: 0.0.3
+Version: 0.0.4
 Summary: Convenient wrapper for executing codes on AWS for connecting and fetching credentials from vault
 Home-page: 
 Download-URL: 
 Author: Mallikarjuna Devaraya
 License: MIT
 Keywords: Vault Credential Fetch,Credential Fetch,Vault
 Classifier: Development Status :: 4 - Beta
```

### Comparing `SecretManagerCredentials-0.0.3/setup.py` & `SecretManagerCredentials-0.0.4/setup.py`

 * *Files identical despite different names*

