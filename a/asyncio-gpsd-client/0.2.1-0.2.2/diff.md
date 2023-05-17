# Comparing `tmp/asyncio-gpsd-client-0.2.1.tar.gz` & `tmp/asyncio_gpsd_client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncio-gpsd-client-0.2.1.tar", max compression
+gzip compressed data, was "asyncio_gpsd_client-0.2.2.tar", max compression
```

## Comparing `asyncio-gpsd-client-0.2.1.tar` & `asyncio_gpsd_client-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1070 2022-09-25 09:39:28.486700 asyncio-gpsd-client-0.2.1/LICENSE
--rw-r--r--   0        0        0      436 2022-09-25 09:39:28.486700 asyncio-gpsd-client-0.2.1/README.md
--rw-r--r--   0        0        0       76 2022-09-25 09:39:28.486700 asyncio-gpsd-client-0.2.1/asyncio_gpsd_client/__init__.py
--rw-r--r--   0        0        0     1925 2022-09-25 09:39:28.486700 asyncio-gpsd-client-0.2.1/asyncio_gpsd_client/client.py
--rw-r--r--   0        0        0       43 2022-09-25 09:39:28.486700 asyncio-gpsd-client-0.2.1/asyncio_gpsd_client/exceptions.py
--rw-r--r--   0        0        0     2204 2022-09-25 09:39:28.486700 asyncio-gpsd-client-0.2.1/asyncio_gpsd_client/schemas.py
--rw-r--r--   0        0        0      696 2022-09-25 09:39:28.486700 asyncio-gpsd-client-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 asyncio-gpsd-client-0.2.1/setup.py
--rw-r--r--   0        0        0      944 1970-01-01 00:00:00.000000 asyncio-gpsd-client-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-17 04:09:59.821246 asyncio_gpsd_client-0.2.2/LICENSE
+-rw-r--r--   0        0        0      436 2023-05-17 04:09:59.821246 asyncio_gpsd_client-0.2.2/README.md
+-rw-r--r--   0        0        0       76 2023-05-17 04:09:59.821246 asyncio_gpsd_client-0.2.2/asyncio_gpsd_client/__init__.py
+-rw-r--r--   0        0        0     1925 2023-05-17 04:09:59.821246 asyncio_gpsd_client-0.2.2/asyncio_gpsd_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-17 04:09:59.821246 asyncio_gpsd_client-0.2.2/asyncio_gpsd_client/exceptions.py
+-rw-r--r--   0        0        0     2204 2023-05-17 04:09:59.821246 asyncio_gpsd_client-0.2.2/asyncio_gpsd_client/schemas.py
+-rw-r--r--   0        0        0      673 2023-05-17 04:09:59.821246 asyncio_gpsd_client-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 asyncio_gpsd_client-0.2.2/PKG-INFO
```

### Comparing `asyncio-gpsd-client-0.2.1/LICENSE` & `asyncio_gpsd_client-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncio-gpsd-client-0.2.1/asyncio_gpsd_client/client.py` & `asyncio_gpsd_client-0.2.2/asyncio_gpsd_client/client.py`

 * *Files identical despite different names*

### Comparing `asyncio-gpsd-client-0.2.1/asyncio_gpsd_client/schemas.py` & `asyncio_gpsd_client-0.2.2/asyncio_gpsd_client/schemas.py`

 * *Files identical despite different names*

### Comparing `asyncio-gpsd-client-0.2.1/PKG-INFO` & `asyncio_gpsd_client-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: asyncio-gpsd-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: asyncio compatible gpsd client
 License: MIT
 Author: Zachary Juang
 Author-email: zachary822@me.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Project-URL: repository, https://github.com/zachary822/asyncio-gpsd-client
 Description-Content-Type: text/markdown
 
 # Asycio Gpsd Client
 
 # Install
```

