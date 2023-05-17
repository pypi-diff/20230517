# Comparing `tmp/douze-0.1.6.tar.gz` & `tmp/douze-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "douze-0.1.6.tar", max compression
+gzip compressed data, was "douze-0.1.7.tar", max compression
```

## Comparing `douze-0.1.6.tar` & `douze-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      484 2020-07-17 09:28:21.000000 douze-0.1.6/LICENSE
--rw-r--r--   0        0        0      254 2020-07-17 09:28:22.000000 douze-0.1.6/README.md
--rw-r--r--   0        0        0      429 2022-06-13 16:10:22.116492 douze-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2020-07-17 09:28:22.000000 douze-0.1.6/src/douze/__init__.py
--rw-r--r--   0        0        0     8548 2022-06-13 16:10:09.359810 douze-0.1.6/src/douze/api.py
--rw-r--r--   0        0        0    17708 2022-06-13 16:10:09.359810 douze-0.1.6/src/douze/idem_api.py
--rw-r--r--   0        0        0     5970 2022-05-03 09:36:26.410142 douze-0.1.6/src/douze/models.py
--rw-r--r--   0        0        0     2803 2022-05-03 09:34:04.400798 douze-0.1.6/src/douze/types.py
--rw-r--r--   0        0        0      966 2022-06-13 16:10:38.315861 douze-0.1.6/setup.py
--rw-r--r--   0        0        0      803 2022-06-13 16:10:38.316293 douze-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      484 2020-07-17 09:28:21.000000 douze-0.1.7/LICENSE
+-rw-r--r--   0        0        0      254 2020-07-17 09:28:22.000000 douze-0.1.7/README.md
+-rw-r--r--   0        0        0      429 2023-05-17 07:46:39.078184 douze-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-07-17 09:28:22.000000 douze-0.1.7/src/douze/__init__.py
+-rw-r--r--   0        0        0     8548 2022-06-13 16:11:22.000000 douze-0.1.7/src/douze/api.py
+-rw-r--r--   0        0        0    17695 2023-05-17 07:43:53.034807 douze-0.1.7/src/douze/idem_api.py
+-rw-r--r--   0        0        0     5970 2022-05-03 09:36:26.000000 douze-0.1.7/src/douze/models.py
+-rw-r--r--   0        0        0     2803 2022-05-03 09:34:04.000000 douze-0.1.7/src/douze/types.py
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 douze-0.1.7/PKG-INFO
```

### Comparing `douze-0.1.6/src/douze/api.py` & `douze-0.1.7/src/douze/api.py`

 * *Files identical despite different names*

### Comparing `douze-0.1.6/src/douze/idem_api.py` & `douze-0.1.7/src/douze/idem_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     def _get_public_ipv4(self) -> Text:
         """
         Tries to figure out your public IPv4, this is helpful to gain temporary
         access to the firewall in order to copy the databases by example.
         """
 
         with Client() as c:
-            return c.get("https://httpbin.org/get").json()["origin"]
+            return c.get('https://api.ipify.org/').text
 
     @contextmanager
     def _allow_self_access(self, cluster_name: Text):
         """
         That's a context manager which will make sure that your IP address is
         allowed in the cluster's firewall during the context.
```

### Comparing `douze-0.1.6/src/douze/models.py` & `douze-0.1.7/src/douze/models.py`

 * *Files identical despite different names*

### Comparing `douze-0.1.6/src/douze/types.py` & `douze-0.1.7/src/douze/types.py`

 * *Files identical despite different names*

### Comparing `douze-0.1.6/PKG-INFO` & `douze-0.1.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: douze
-Version: 0.1.6
+Version: 0.1.7
 Summary: A DigitalOcean API client to help with 12-factors apps
 License: WTFPL
 Author: Rémy Sanchez
 Author-email: remy.sanchez@hyperthese.net
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: typefit (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown
 
 DOuze
 =====
 
 A DigitalOcean client library aimed to be a backend for Ansible modules.
```

