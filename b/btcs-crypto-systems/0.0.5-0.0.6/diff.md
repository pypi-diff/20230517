# Comparing `tmp/btcs_crypto_systems-0.0.5.tar.gz` & `tmp/btcs_crypto_systems-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btcs_crypto_systems-0.0.5.tar", last modified: Wed May 17 06:44:09 2023, max compression
+gzip compressed data, was "btcs_crypto_systems-0.0.6.tar", last modified: Wed May 17 11:03:48 2023, max compression
```

## Comparing `btcs_crypto_systems-0.0.5.tar` & `btcs_crypto_systems-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 06:44:09.501103 btcs_crypto_systems-0.0.5/
--rw-rw-rw-   0        0        0     1338 2023-05-17 06:44:09.499101 btcs_crypto_systems-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1157 2023-02-17 09:17:57.000000 btcs_crypto_systems-0.0.5/README.md
--rw-rw-rw-   0        0        0      176 2023-05-17 06:43:55.000000 btcs_crypto_systems-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-17 06:44:09.501103 btcs_crypto_systems-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-17 06:44:09.455122 btcs_crypto_systems-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-17 06:44:09.480104 btcs_crypto_systems-0.0.5/src/btcs_crypto_systems/
--rw-rw-rw-   0        0        0        0 2023-05-17 06:42:37.000000 btcs_crypto_systems-0.0.5/src/btcs_crypto_systems/__init__.py
--rw-rw-rw-   0        0        0     1267 2023-02-17 09:08:56.000000 btcs_crypto_systems-0.0.5/src/btcs_crypto_systems/address_manangement_service.py
--rw-rw-rw-   0        0        0     9621 2023-05-17 06:43:30.000000 btcs_crypto_systems-0.0.5/src/btcs_crypto_systems/token_master.py
--rw-rw-rw-   0        0        0      348 2023-02-17 08:38:32.000000 btcs_crypto_systems-0.0.5/src/btcs_crypto_systems/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 06:44:09.496104 btcs_crypto_systems-0.0.5/src/btcs_crypto_systems.egg-info/
--rw-rw-rw-   0        0        0     1338 2023-05-17 06:44:09.000000 btcs_crypto_systems-0.0.5/src/btcs_crypto_systems.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-05-17 06:44:09.000000 btcs_crypto_systems-0.0.5/src/btcs_crypto_systems.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 06:44:09.000000 btcs_crypto_systems-0.0.5/src/btcs_crypto_systems.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-17 06:44:09.000000 btcs_crypto_systems-0.0.5/src/btcs_crypto_systems.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 11:03:48.266706 btcs_crypto_systems-0.0.6/
+-rw-rw-rw-   0        0        0     1338 2023-05-17 11:03:48.264695 btcs_crypto_systems-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1157 2023-02-17 09:17:57.000000 btcs_crypto_systems-0.0.6/README.md
+-rw-rw-rw-   0        0        0      176 2023-05-17 09:30:29.000000 btcs_crypto_systems-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-17 11:03:48.266706 btcs_crypto_systems-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 11:03:48.190120 btcs_crypto_systems-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-17 11:03:48.232125 btcs_crypto_systems-0.0.6/src/btcs_crypto_systems/
+-rw-rw-rw-   0        0        0        0 2023-05-17 06:42:37.000000 btcs_crypto_systems-0.0.6/src/btcs_crypto_systems/__init__.py
+-rw-rw-rw-   0        0        0     1267 2023-02-17 09:08:56.000000 btcs_crypto_systems-0.0.6/src/btcs_crypto_systems/address_manangement_service.py
+-rw-rw-rw-   0        0        0    17614 2023-05-17 11:01:50.000000 btcs_crypto_systems-0.0.6/src/btcs_crypto_systems/token_master.py
+-rw-rw-rw-   0        0        0      348 2023-02-17 08:38:32.000000 btcs_crypto_systems-0.0.6/src/btcs_crypto_systems/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:03:48.256710 btcs_crypto_systems-0.0.6/src/btcs_crypto_systems.egg-info/
+-rw-rw-rw-   0        0        0     1338 2023-05-17 11:03:48.000000 btcs_crypto_systems-0.0.6/src/btcs_crypto_systems.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-05-17 11:03:48.000000 btcs_crypto_systems-0.0.6/src/btcs_crypto_systems.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 11:03:48.000000 btcs_crypto_systems-0.0.6/src/btcs_crypto_systems.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-17 11:03:48.000000 btcs_crypto_systems-0.0.6/src/btcs_crypto_systems.egg-info/top_level.txt
```

### Comparing `btcs_crypto_systems-0.0.5/PKG-INFO` & `btcs_crypto_systems-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btcs_crypto_systems
-Version: 0.0.5
+Version: 0.0.6
 Summary: To interact with BTCS crypto systems.
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # crypto systems package for BTCS crypto business systems
```

### Comparing `btcs_crypto_systems-0.0.5/README.md` & `btcs_crypto_systems-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `btcs_crypto_systems-0.0.5/src/btcs_crypto_systems/address_manangement_service.py` & `btcs_crypto_systems-0.0.6/src/btcs_crypto_systems/address_manangement_service.py`

 * *Files identical despite different names*

### Comparing `btcs_crypto_systems-0.0.5/src/btcs_crypto_systems.egg-info/PKG-INFO` & `btcs_crypto_systems-0.0.6/src/btcs_crypto_systems.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btcs-crypto-systems
-Version: 0.0.5
+Version: 0.0.6
 Summary: To interact with BTCS crypto systems.
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # crypto systems package for BTCS crypto business systems
```

