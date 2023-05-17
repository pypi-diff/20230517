# Comparing `tmp/mse_lib_sgx-2.0a1.tar.gz` & `tmp/mse_lib_sgx-2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mse_lib_sgx-2.0a1.tar", last modified: Wed May 17 13:00:08 2023, max compression
+gzip compressed data, was "mse_lib_sgx-2.0a2.tar", last modified: Wed May 17 14:25:19 2023, max compression
```

## Comparing `mse_lib_sgx-2.0a1.tar` & `mse_lib_sgx-2.0a2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:08.535043 mse_lib_sgx-2.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-17 13:00:08.535043 mse_lib_sgx-2.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-17 13:00:08.535043 mse_lib_sgx-2.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:08.531043 mse_lib_sgx-2.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:08.535043 mse_lib_sgx-2.0a1/src/mse_lib_sgx/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/base64url.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/globs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/http_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/import_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:08.535043 mse_lib_sgx-2.0a1/src/mse_lib_sgx/sgx/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/sgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/sgx/key.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/sgx/quote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:08.535043 mse_lib_sgx-2.0a1/src/mse_lib_sgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-17 13:00:08.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-17 13:00:08.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:00:08.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 13:00:08.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:00:08.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-17 13:00:08.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 13:00:08.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:08.535043 mse_lib_sgx-2.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/tests/test_cert_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/tests/test_conf_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:25:19.207008 mse_lib_sgx-2.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-17 14:25:19.207008 mse_lib_sgx-2.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-17 14:25:19.207008 mse_lib_sgx-2.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:25:19.207008 mse_lib_sgx-2.0a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:25:19.207008 mse_lib_sgx-2.0a2/src/mse_lib_sgx/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/base64url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/globs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/http_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/import_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:25:19.207008 mse_lib_sgx-2.0a2/src/mse_lib_sgx/sgx/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/sgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/sgx/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/sgx/quote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:25:19.207008 mse_lib_sgx-2.0a2/src/mse_lib_sgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-17 14:25:19.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-17 14:25:19.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:25:19.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 14:25:19.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:25:19.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-17 14:25:19.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 14:25:19.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:25:19.207008 mse_lib_sgx-2.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/tests/test_cert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/tests/test_conf_server.py
```

### Comparing `mse_lib_sgx-2.0a1/PKG-INFO` & `mse_lib_sgx-2.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse_lib_sgx
-Version: 2.0a1
+Version: 2.0a2
 Summary: Library for Cosmian MSE to bootstrap Flask application
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mse_lib_sgx-2.0a1/README.md` & `mse_lib_sgx-2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a1/setup.py` & `mse_lib_sgx-2.0a2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     packages=find_packages("src"),
     package_dir={"": "src"},
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     zip_safe=False,
     install_requires=[
         "cryptography>=40.0.2,<40.1.0",
-        "intel-sgx-ra==2.0a2",
+        "intel-sgx-ra==2.0a3",
         "hypercorn[uvloop]>=0.14.3,<0.15.0",
         "h2>=4.1.0,<4.2.0",
         "mse-lib-crypto>=1.2,<2.0",
     ],
     entry_points={
         "console_scripts": ["mse-bootstrap = mse_lib_sgx.cli:run"],
     },
```

### Comparing `mse_lib_sgx-2.0a1/src/mse_lib_sgx/base64url.py` & `mse_lib_sgx-2.0a2/src/mse_lib_sgx/base64url.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a1/src/mse_lib_sgx/certificate.py` & `mse_lib_sgx-2.0a2/src/mse_lib_sgx/certificate.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a1/src/mse_lib_sgx/cli.py` & `mse_lib_sgx-2.0a2/src/mse_lib_sgx/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,18 +75,18 @@
     parser.add_argument(
         "--debug", action="store_true", help="debug mode with more logging"
     )
 
     group = parser.add_mutually_exclusive_group(required=True)
 
     group.add_argument(
-        "--self-signed",
+        "--ratls",
         type=int,
         metavar="EXPIRATION_DATE",
-        help="generate a self-signed certificate for the web app with a "
+        help="generate a self-signed certificate for RA-TLS with a "
         "specific expiration date (Unix time)",
     )
 
     group.add_argument("--no-ssl", action="store_true", help="use HTTP without SSL")
 
     group.add_argument(
         "--certificate",
@@ -156,15 +156,15 @@
         # The conf server use the self-signed cert
         # The app server use the app owner cert
         ssl_app_mode = SslAppMode.CUSTOM_CERTIFICATE
         ssl_private_key_path = globs.KEY_DIR_PATH / "key.pem"
     else:
         # The conf server and the app server will use the same self-signed cert
         ssl_app_mode = SslAppMode.RATLS_CERTIFICATE
-        expiration_date = datetime.utcfromtimestamp(args.self_signed)
+        expiration_date = datetime.utcfromtimestamp(args.ratls)
 
     logging.info("Generating self-signed certificate...")
 
     if not globs.ENCLAVE_SK_PATH.exists():
         globs.ENCLAVE_SK_PATH.write_bytes(get_mrenclave_key())
 
     enclave_pk: bytes = x25519_pk_from_sk(globs.ENCLAVE_SK_PATH.read_bytes())
```

### Comparing `mse_lib_sgx-2.0a1/src/mse_lib_sgx/globs.py` & `mse_lib_sgx-2.0a2/src/mse_lib_sgx/globs.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a1/src/mse_lib_sgx/http_server.py` & `mse_lib_sgx-2.0a2/src/mse_lib_sgx/http_server.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a1/src/mse_lib_sgx/import_hook.py` & `mse_lib_sgx-2.0a2/src/mse_lib_sgx/import_hook.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a1/src/mse_lib_sgx/sgx/key.py` & `mse_lib_sgx-2.0a2/src/mse_lib_sgx/sgx/key.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a1/src/mse_lib_sgx/sgx/quote.py` & `mse_lib_sgx-2.0a2/src/mse_lib_sgx/sgx/quote.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a1/src/mse_lib_sgx.egg-info/PKG-INFO` & `mse_lib_sgx-2.0a2/src/mse_lib_sgx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse-lib-sgx
-Version: 2.0a1
+Version: 2.0a2
 Summary: Library for Cosmian MSE to bootstrap Flask application
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mse_lib_sgx-2.0a1/src/mse_lib_sgx.egg-info/SOURCES.txt` & `mse_lib_sgx-2.0a2/src/mse_lib_sgx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a1/tests/test_cert_utils.py` & `mse_lib_sgx-2.0a2/tests/test_cert_utils.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a1/tests/test_conf_server.py` & `mse_lib_sgx-2.0a2/tests/test_conf_server.py`

 * *Files identical despite different names*

