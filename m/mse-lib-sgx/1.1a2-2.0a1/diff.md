# Comparing `tmp/mse_lib_sgx-1.1a2.tar.gz` & `tmp/mse_lib_sgx-2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mse_lib_sgx-1.1a2.tar", last modified: Thu Feb 16 16:26:14 2023, max compression
+gzip compressed data, was "mse_lib_sgx-2.0a1.tar", last modified: Wed May 17 13:00:08 2023, max compression
```

## Comparing `mse_lib_sgx-1.1a2.tar` & `mse_lib_sgx-2.0a1.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:26:14.620138 mse_lib_sgx-1.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-02-16 16:26:14.620138 mse_lib_sgx-1.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-02-16 16:25:30.000000 mse_lib_sgx-1.1a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-02-16 16:26:14.620138 mse_lib_sgx-1.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-02-16 16:25:30.000000 mse_lib_sgx-1.1a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:26:14.616137 mse_lib_sgx-1.1a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:26:14.620138 mse_lib_sgx-1.1a2/src/mse_lib_sgx/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-16 16:25:30.000000 mse_lib_sgx-1.1a2/src/mse_lib_sgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-02-16 16:25:30.000000 mse_lib_sgx-1.1a2/src/mse_lib_sgx/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-02-16 16:25:30.000000 mse_lib_sgx-1.1a2/src/mse_lib_sgx/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-02-16 16:25:30.000000 mse_lib_sgx-1.1a2/src/mse_lib_sgx/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-02-16 16:25:30.000000 mse_lib_sgx-1.1a2/src/mse_lib_sgx/globs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-02-16 16:25:30.000000 mse_lib_sgx-1.1a2/src/mse_lib_sgx/http_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-02-16 16:25:30.000000 mse_lib_sgx-1.1a2/src/mse_lib_sgx/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-02-16 16:25:30.000000 mse_lib_sgx-1.1a2/src/mse_lib_sgx/sgx_quote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:26:14.620138 mse_lib_sgx-1.1a2/src/mse_lib_sgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-02-16 16:26:14.000000 mse_lib_sgx-1.1a2/src/mse_lib_sgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-02-16 16:26:14.000000 mse_lib_sgx-1.1a2/src/mse_lib_sgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 16:26:14.000000 mse_lib_sgx-1.1a2/src/mse_lib_sgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-16 16:26:14.000000 mse_lib_sgx-1.1a2/src/mse_lib_sgx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 16:26:14.000000 mse_lib_sgx-1.1a2/src/mse_lib_sgx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-16 16:26:14.000000 mse_lib_sgx-1.1a2/src/mse_lib_sgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-16 16:26:14.000000 mse_lib_sgx-1.1a2/src/mse_lib_sgx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:26:14.620138 mse_lib_sgx-1.1a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-02-16 16:25:30.000000 mse_lib_sgx-1.1a2/tests/test_cert_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-02-16 16:25:30.000000 mse_lib_sgx-1.1a2/tests/test_conf_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:08.535043 mse_lib_sgx-2.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-17 13:00:08.535043 mse_lib_sgx-2.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-17 13:00:08.535043 mse_lib_sgx-2.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:08.531043 mse_lib_sgx-2.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:08.535043 mse_lib_sgx-2.0a1/src/mse_lib_sgx/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/base64url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/globs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/http_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/import_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:08.535043 mse_lib_sgx-2.0a1/src/mse_lib_sgx/sgx/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/sgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/sgx/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx/sgx/quote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:08.535043 mse_lib_sgx-2.0a1/src/mse_lib_sgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-17 13:00:08.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-17 13:00:08.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:00:08.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 13:00:08.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:00:08.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-17 13:00:08.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 13:00:08.000000 mse_lib_sgx-2.0a1/src/mse_lib_sgx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:08.535043 mse_lib_sgx-2.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/tests/test_cert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-17 12:59:13.000000 mse_lib_sgx-2.0a1/tests/test_conf_server.py
```

### Comparing `mse_lib_sgx-1.1a2/PKG-INFO` & `mse_lib_sgx-2.0a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse_lib_sgx
-Version: 1.1a2
+Version: 2.0a1
 Summary: Library for Cosmian MSE to bootstrap Flask application
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -43,35 +43,36 @@
 $ pip install mse-lib-sgx
 ```
 
 ## Usage
 
 ```console
 $ mse-bootstrap --help
-usage: mse-bootstrap [-h] --host HOST --port PORT --app-dir APP_DIR --uuid UUID [--version]
-                     [--debug]
+usage: mse-bootstrap [-h] --host HOST --port PORT --app-dir APP_DIR --uuid
+                     UUID [--version] [--debug]
                      (--self-signed EXPIRATION_DATE | --no-ssl | --certificate CERTIFICATE_PATH)
                      application
 
 Bootstrap ASGI/WSGI Python web application for Gramine
 
 positional arguments:
-  application           Application to dispatch to as path.to.module:instance.path
+  application           ASGI application path (as module:app)
 
 optional arguments:
   -h, --help            show this help message and exit
-  --host HOST           Hostname of the configuration serverIf `--self-signed`, it's also the
-                        hostname of the app server
-  --port PORT           Port of the server
-  --app-dir APP_DIR     Path the microservice application. Read only directory.
-  --uuid UUID           Unique application UUID.
+  --host HOST           hostname of the configuration server, also the
+                        hostname of the app server if `--self-signed`
+  --port PORT           port of the server
+  --app-dir APP_DIR     path of the python web application
+  --uuid UUID           unique application UUID
   --version             show program's version number and exit
-  --debug               Debug mode without SGX
+  --debug               debug mode with more logging
   --self-signed EXPIRATION_DATE
-                        Generate a self-signed certificate for the app. Specify the expiration
-                        date of the certificate as a timestamp since Epoch
-  --no-ssl              Don't use HTTPS connection
+                        generate a self-signed certificate for the web app
+                        with a specific expiration date (Unix time)
+  --no-ssl              use HTTP without SSL
   --certificate CERTIFICATE_PATH
-                        Use the given certificate for the SSL connection. the private key will
-                        be sent using the configuration server
+                        custom certificate used for the SSL connection,
+                        private key must be sent through the configuration
+                        server
 
 ```
```

### Comparing `mse_lib_sgx-1.1a2/README.md` & `mse_lib_sgx-2.0a1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -30,35 +30,36 @@
 $ pip install mse-lib-sgx
 ```
 
 ## Usage
 
 ```console
 $ mse-bootstrap --help
-usage: mse-bootstrap [-h] --host HOST --port PORT --app-dir APP_DIR --uuid UUID [--version]
-                     [--debug]
+usage: mse-bootstrap [-h] --host HOST --port PORT --app-dir APP_DIR --uuid
+                     UUID [--version] [--debug]
                      (--self-signed EXPIRATION_DATE | --no-ssl | --certificate CERTIFICATE_PATH)
                      application
 
 Bootstrap ASGI/WSGI Python web application for Gramine
 
 positional arguments:
-  application           Application to dispatch to as path.to.module:instance.path
+  application           ASGI application path (as module:app)
 
 optional arguments:
   -h, --help            show this help message and exit
-  --host HOST           Hostname of the configuration serverIf `--self-signed`, it's also the
-                        hostname of the app server
-  --port PORT           Port of the server
-  --app-dir APP_DIR     Path the microservice application. Read only directory.
-  --uuid UUID           Unique application UUID.
+  --host HOST           hostname of the configuration server, also the
+                        hostname of the app server if `--self-signed`
+  --port PORT           port of the server
+  --app-dir APP_DIR     path of the python web application
+  --uuid UUID           unique application UUID
   --version             show program's version number and exit
-  --debug               Debug mode without SGX
+  --debug               debug mode with more logging
   --self-signed EXPIRATION_DATE
-                        Generate a self-signed certificate for the app. Specify the expiration
-                        date of the certificate as a timestamp since Epoch
-  --no-ssl              Don't use HTTPS connection
+                        generate a self-signed certificate for the web app
+                        with a specific expiration date (Unix time)
+  --no-ssl              use HTTP without SSL
   --certificate CERTIFICATE_PATH
-                        Use the given certificate for the SSL connection. the private key will
-                        be sent using the configuration server
+                        custom certificate used for the SSL connection,
+                        private key must be sent through the configuration
+                        server
 
 ```
```

### Comparing `mse_lib_sgx-1.1a2/setup.py` & `mse_lib_sgx-2.0a1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,19 +29,19 @@
     description="Library for Cosmian MSE to bootstrap Flask application",
     packages=find_packages("src"),
     package_dir={"": "src"},
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     zip_safe=False,
     install_requires=[
-        "cryptography>=39.0.0,<40.0.0",
-        "intel-sgx-ra>=1.0,<1.1",
+        "cryptography>=40.0.2,<40.1.0",
+        "intel-sgx-ra==2.0a2",
         "hypercorn[uvloop]>=0.14.3,<0.15.0",
         "h2>=4.1.0,<4.2.0",
-        "mse-lib-crypto>=1.1,<1.2",
+        "mse-lib-crypto>=1.2,<2.0",
     ],
     entry_points={
         "console_scripts": ["mse-bootstrap = mse_lib_sgx.cli:run"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `mse_lib_sgx-1.1a2/src/mse_lib_sgx/certificate.py` & `mse_lib_sgx-2.0a1/src/mse_lib_sgx/certificate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """mse_lib_sgx.certificate module."""
 
 import hashlib
+import ipaddress
 from datetime import datetime
 from pathlib import Path
-from typing import List, Optional, cast
+from typing import List, Optional, Union, cast
 from urllib.parse import urlparse
 
 from cryptography import x509
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.hazmat.primitives.serialization import (
     Encoding,
@@ -15,27 +16,27 @@
     PrivateFormat,
     PublicFormat,
     load_pem_private_key,
 )
 from intel_sgx_ra.quote import Quote
 from intel_sgx_ra.ratls import SGX_QUOTE_EXTENSION_OID, get_quote_from_cert
 
-from mse_lib_sgx.sgx_quote import get_quote
+from mse_lib_sgx.sgx.quote import get_quote
 
 
 class Certificate:
     """Certificate class."""
 
     def __init__(
         self,
-        dns_name: str,
+        subject_alternative_name: str,
         subject: x509.Name,
         root_path: Path,
         expiration_date: datetime,
-        ratls: bool = True,
+        ratls: Optional[bytes],
     ):
         """Init constructor of SGXCertificate."""
         self.cert_path: Path = root_path / "cert.ratls.pem"
         self.key_path: Path = root_path / "key.ratls.pem"
         self.sk: ec.EllipticCurvePrivateKey = (
             ec.generate_private_key(curve=ec.SECP256R1())
             if not self.key_path.exists()
@@ -45,34 +46,36 @@
             )
         )
         self.expiration_date: datetime = expiration_date
         self.cert: x509.Certificate
         self.quote: Optional[Quote] = None
         if self.key_path.exists() and self.cert_path.exists():
             self.cert = x509.load_pem_x509_certificate(data=self.cert_path.read_bytes())
-            if ratls:
+            if ratls is not None:
                 self.quote = get_quote_from_cert(self.cert)
         else:
             custom_extension: Optional[x509.ExtensionType] = None
-            if ratls:
-                self.quote = Quote.from_bytes(
-                    get_quote(
-                        user_report_data=hashlib.sha256(
-                            self.sk.public_key().public_bytes(
-                                encoding=Encoding.X962,
-                                format=PublicFormat.UncompressedPoint,
-                            )
-                        ).digest()
+            if ratls is not None:
+                pubkey_hash: bytes = hashlib.sha256(
+                    self.sk.public_key().public_bytes(
+                        encoding=Encoding.X962,
+                        format=PublicFormat.UncompressedPoint,
                     )
+                ).digest()
+                user_report_data: bytes = (
+                    pubkey_hash + ratls if ratls is not None else pubkey_hash
+                )
+                self.quote = Quote.from_bytes(
+                    get_quote(user_report_data=user_report_data)
                 )
                 custom_extension = x509.UnrecognizedExtension(
                     oid=SGX_QUOTE_EXTENSION_OID, value=bytes(self.quote)
                 )
             self.cert = generate_x509(
-                dns_name=dns_name,
+                subject_alternative_name=subject_alternative_name,
                 subject=subject,
                 private_key=self.sk,
                 expiration_date=self.expiration_date,
                 custom_extension=custom_extension,
             )
             self.write(self.cert_path, self.key_path)
 
@@ -87,34 +90,40 @@
                 format=PrivateFormat.PKCS8,
                 encryption_algorithm=NoEncryption(),
             )
         )
 
 
 def generate_x509(
-    dns_name: str,
+    subject_alternative_name: str,
     subject: x509.Name,
     private_key: ec.EllipticCurvePrivateKey,
     expiration_date: datetime,
     custom_extension: Optional[x509.ExtensionType] = None,
 ) -> x509.Certificate:
     """X509 certificate generation."""
     issuer: x509.Name = subject  # issuer=subject for self-signed certificate
 
+    san: Union[x509.IPAddress, x509.DNSName]
+    try:
+        san = x509.IPAddress(ipaddress.ip_address(subject_alternative_name))
+    except ValueError:
+        san = x509.DNSName(subject_alternative_name)
+
     builder: x509.CertificateBuilder = x509.CertificateBuilder()
 
     builder = (
         builder.subject_name(subject)
         .issuer_name(issuer)
         .public_key(private_key.public_key())
         .serial_number(x509.random_serial_number())
         .not_valid_before(datetime.utcnow())
         .not_valid_after(expiration_date)
         .add_extension(
-            x509.SubjectAlternativeName([x509.DNSName(dns_name)]),
+            x509.SubjectAlternativeName([san]),
             critical=False,
         )
     )
 
     if custom_extension is not None:
         builder = builder.add_extension(custom_extension, critical=False)
 
@@ -124,16 +133,21 @@
     )
 
     return builder.sign(private_key=private_key, algorithm=hashes.SHA256())
 
 
 def to_wildcard_domain(domain: str) -> str:
     """Add wildcard to first subdomain."""
-    if "." not in domain:
-        return domain
+    try:
+        _ = ipaddress.ip_address(domain)
+    except ValueError:
+        if "." not in domain:
+            return domain
+
+        subdomains: List[str] = urlparse(f"//{domain}").netloc.split(".")
 
-    subdomains: List[str] = urlparse(f"//{domain}").netloc.split(".")
+        if len(subdomains) <= 2:
+            return domain
 
-    if len(subdomains) <= 2:
-        return domain
+        return f"*.{'.'.join(subdomains[1:])}"
 
-    return f"*.{'.'.join(subdomains[1:])}"
+    return domain
```

### Comparing `mse_lib_sgx-1.1a2/src/mse_lib_sgx/cli.py` & `mse_lib_sgx-2.0a1/src/mse_lib_sgx/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,96 +1,117 @@
 """mse_lib_sgx.cli.bootstrap module."""
 
 import argparse
 import asyncio
 import importlib
 import logging
+import shutil
 import sys
 import sysconfig
+import uuid
 from datetime import datetime, timedelta
 from enum import Enum
 from pathlib import Path
 
+from cryptography import x509
 from hypercorn.asyncio import serve
 from hypercorn.config import Config
+from mse_lib_crypto.x25519 import x25519_pk_from_sk
 from mse_lib_crypto.xsalsa20_poly1305 import decrypt_directory
 
 from mse_lib_sgx import __version__, globs
-from mse_lib_sgx.certificate import Certificate, to_wildcard_domain
+from mse_lib_sgx.certificate import Certificate
 from mse_lib_sgx.error import SecurityError
 from mse_lib_sgx.http_server import serve as serve_sgx_secrets
+from mse_lib_sgx.sgx.key import get_mrenclave_key
 
 
 def parse_args() -> argparse.Namespace:
     """Argument parser."""
     parser = argparse.ArgumentParser(
         description="Bootstrap ASGI/WSGI Python web application for Gramine"
     )
     parser.add_argument(
         "application",
         type=str,
-        help="Application to dispatch to as path.to.module:instance.path",
+        help="ASGI application path (as module:app)",
     )
 
     parser.add_argument(
         "--host",
-        required=True,
         type=str,
-        help="Hostname of the configuration server"
-        "If `--self-signed`, it's also the hostname of the app server",
+        default="0.0.0.0",
+        help="hostname of the server",
+    )
+    parser.add_argument("--port", type=int, default=443, help="port of the server")
+    parser.add_argument(
+        "--subject",
+        type=str,
+        help="Subject as RFC 4514 string for the RA-TLS certificate",
+    )
+    parser.add_argument(
+        "--san", type=str, help="Subject Alternative Name in the RA-TLS certificate"
     )
-    parser.add_argument("--port", required=True, type=int, help="Port of the server")
     parser.add_argument(
         "--app-dir",
         required=True,
         type=Path,
-        help="Path of the microservice application. Read only directory.",
+        help="path of the python web application",
     )
     parser.add_argument(
-        "--uuid", required=True, type=str, help="Unique application UUID."
+        "--id",
+        required=True,
+        type=uuid.UUID,
+        help="identifier of the application as UUID in RFC 4122",
+    )
+    parser.add_argument(
+        "--plaincode", action="store_true", help="unencrypted python web application"
+    )
+    parser.add_argument(
+        "--timeout", type=int, help="seconds before closing the configuration server"
     )
     parser.add_argument(
         "--version", action="version", version=f"%(prog)s {__version__}"
     )
-    parser.add_argument("--debug", action="store_true", help="Debug mode without SGX")
+    parser.add_argument(
+        "--debug", action="store_true", help="debug mode with more logging"
+    )
 
     group = parser.add_mutually_exclusive_group(required=True)
 
     group.add_argument(
         "--self-signed",
         type=int,
         metavar="EXPIRATION_DATE",
-        help="Generate a self-signed certificate for the app. "
-        "Specify the expiration date of the certificate "
-        "as a timestamp since Epoch",
+        help="generate a self-signed certificate for the web app with a "
+        "specific expiration date (Unix time)",
     )
 
-    group.add_argument(
-        "--no-ssl", action="store_true", help="Don't use HTTPS connection"
-    )
+    group.add_argument("--no-ssl", action="store_true", help="use HTTP without SSL")
 
     group.add_argument(
         "--certificate",
         type=Path,
         metavar="CERTIFICATE_PATH",
-        help="Use the given certificate for the SSL connection. "
-        "the private key will be sent using the configuration server",
+        help="custom certificate used for the SSL connection, "
+        "private key must be sent through the configuration server",
     )
 
     return parser.parse_args()
 
 
 class SslAppMode(Enum):
     """SSL Application Mode."""
 
     RATLS_CERTIFICATE = 1  # self-signed SGX certificate with quote
     CUSTOM_CERTIFICATE = 2  # provided by the code provider
     NO_SSL = 3  # no SSL, will be done by the SSL proxy
 
 
+# pylint: disable=too-many-statements,too-many-branches
 def run() -> None:
     """Entrypoint of the CLI.
 
     The program creates a self-signed certificate.
 
     Then starts a configuration server using HTTPS and this previous cert
     in order to allow the user to send some secrets params.
@@ -109,23 +130,26 @@
     args: argparse.Namespace = parse_args()
 
     globs.HOME_DIR_PATH.mkdir(exist_ok=True)
     globs.KEY_DIR_PATH.mkdir(exist_ok=True)
     globs.MODULE_DIR_PATH.mkdir(exist_ok=True)
 
     logging.basicConfig(
-        level=logging.INFO, format="[%(asctime)s] [%(levelname)s] %(message)s"
+        level=logging.DEBUG if args.debug else logging.INFO,
+        format="[%(asctime)s] [%(levelname)s] %(message)s",
     )
 
+    if args.plaincode:
+        globs.PLAINCODE = True
+
+    if args.timeout:
+        globs.TIMEOUT = args.timeout
+
     ssl_private_key_path = None
     expiration_date = datetime.now() + timedelta(hours=10)
-    common_name: str = to_wildcard_domain(args.host)
-
-    if not common_name:
-        raise SecurityError(f"Can't parse host to extract Common Name: {args.host}")
 
     ssl_app_mode: SslAppMode
     if args.no_ssl:
         # The conf server use the self-signed cert
         # No ssl for the app server
         ssl_app_mode = SslAppMode.NO_SSL
     elif args.certificate:
@@ -136,60 +160,74 @@
     else:
         # The conf server and the app server will use the same self-signed cert
         ssl_app_mode = SslAppMode.RATLS_CERTIFICATE
         expiration_date = datetime.utcfromtimestamp(args.self_signed)
 
     logging.info("Generating self-signed certificate...")
 
+    if not globs.ENCLAVE_SK_PATH.exists():
+        globs.ENCLAVE_SK_PATH.write_bytes(get_mrenclave_key())
+
+    enclave_pk: bytes = x25519_pk_from_sk(globs.ENCLAVE_SK_PATH.read_bytes())
+
+    if len(enclave_pk) != 32:
+        raise SecurityError("Bad enclave pk length!")
+
     cert: Certificate = Certificate(
-        dns_name=args.host,
-        subject=globs.SUBJECT,
+        subject_alternative_name=args.san if args.san else "localhost",
+        subject=(
+            x509.Name.from_rfc4514_string(args.subject)
+            if args.subject
+            else globs.SUBJECT
+        ),
         root_path=globs.KEY_DIR_PATH,
         expiration_date=expiration_date,
-        ratls=True,
+        ratls=enclave_pk,
     )
 
-    symkey_path: Path = globs.KEY_DIR_PATH / "code.key"
-
-    if not symkey_path.exists():
+    if not globs.CODE_KEY_PATH.exists():
         logging.info("Starting the configuration server...")
         # The app owner will send:
         # - the uuid of the app (see as an uniq token allowing to query the API)
         # - the key to decrypt the code
         # - (optional) the SSL private key if AppConnection.OWNER_CERTFICIATE
         serve_sgx_secrets(
-            hostname="0.0.0.0",
+            hostname=args.host,
             port=args.port,
             certificate=cert,
             uuid=args.uuid,
             need_ssl_private_key=ssl_app_mode == SslAppMode.CUSTOM_CERTIFICATE,
             timeout=globs.TIMEOUT,
         )
 
-        if globs.CODE_SECRET_KEY is None:
-            raise SecurityError("Code secret key not proviced")
+        if not globs.PLAINCODE and globs.CODE_SECRET_KEY is None:
+            raise SecurityError("Code secret key not provided")
 
-        symkey_path.write_bytes(globs.CODE_SECRET_KEY)
+        if not globs.PLAINCODE and globs.CODE_SECRET_KEY is not None:
+            globs.CODE_KEY_PATH.write_bytes(globs.CODE_SECRET_KEY)
 
         if (
             ssl_app_mode == SslAppMode.CUSTOM_CERTIFICATE
             and globs.SSL_PRIVATE_KEY
             and ssl_private_key_path is not None
         ):
             ssl_private_key_path.write_text(globs.SSL_PRIVATE_KEY)
 
-    decrypt_directory(
-        dir_path=args.app_dir,
-        key=symkey_path.read_bytes(),
-        ext=".enc",
-        out_dir_path=globs.MODULE_DIR_PATH,
-    )
+    if globs.PLAINCODE:
+        shutil.copy(args.app_dir, globs.MODULE_DIR_PATH)
+    else:
+        decrypt_directory(
+            dir_path=args.app_dir,
+            key=globs.CODE_KEY_PATH.read_bytes(),
+            ext=".enc",
+            out_dir_path=globs.MODULE_DIR_PATH,
+        )
 
     config_map = {
-        "bind": f"0.0.0.0:{args.port}",
+        "bind": f"{args.host}:{args.port}",
         "alpn_protocols": ["h2"],
         "workers": 1,
         "accesslog": "-",
         "errorlog": "-",
         "worker_class": "uvloop",
         "wsgi_max_body_size": 2 * 1024 * 1024 * 1024,  # 2 GB
     }
```

### Comparing `mse_lib_sgx-1.1a2/src/mse_lib_sgx/globs.py` & `mse_lib_sgx-2.0a1/src/mse_lib_sgx/globs.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,24 +12,31 @@
 
 EXIT_EVENT: threading.Event = threading.Event()
 
 UUID: Optional[str] = None
 
 SSL_PRIVATE_KEY: Optional[str] = None
 NEED_SSL_PRIVATE_KEY: bool = False
+PLAINCODE: bool = False
 
 HOME_DIR_PATH: Path = Path(os.getenv("HOME", "/root"))
 KEY_DIR_PATH: Path = Path(os.getenv("KEY_PATH", "/key"))
 SECRETS_PATH: Path = Path(os.getenv("SECRETS_PATH", "/root/.cache/mse/secrets.json"))
+SEALED_SECRETS_PATH: Path = Path(
+    os.getenv("SEALED_SECRETS_PATH", "/root/.cache/mse/sealed_secrets.json")
+)
 MODULE_DIR_PATH: Path = Path(os.getenv("MODULE_PATH", "/mse-app"))
 
+CODE_KEY_PATH: Path = KEY_DIR_PATH / "code.key"
+ENCLAVE_SK_PATH: Path = KEY_DIR_PATH / "enclave.key"
+
 SUBJECT: x509.Name = x509.Name(
     [
         x509.NameAttribute(NameOID.COUNTRY_NAME, "FR"),
         x509.NameAttribute(NameOID.STATE_OR_PROVINCE_NAME, "Ile-de-France"),
         x509.NameAttribute(NameOID.LOCALITY_NAME, "Paris"),
         x509.NameAttribute(NameOID.ORGANIZATION_NAME, "Cosmian Tech"),
         x509.NameAttribute(NameOID.COMMON_NAME, "localhost"),
     ]
 )
 
-TIMEOUT: int = 180
+TIMEOUT: Optional[int] = None
```

### Comparing `mse_lib_sgx-1.1a2/src/mse_lib_sgx/http_server.py` & `mse_lib_sgx-2.0a1/src/mse_lib_sgx/http_server.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,20 @@
 
 import json
 import logging
 import ssl
 import threading
 import time
 from http.server import BaseHTTPRequestHandler, HTTPServer
+from typing import Optional
+
+from mse_lib_crypto.seal_box import unseal
 
 from mse_lib_sgx import globs
+from mse_lib_sgx.base64url import base64url_decode
 from mse_lib_sgx.certificate import Certificate
 from mse_lib_sgx.error import CryptoError
 
 
 class SGXHTTPRequestHandler(BaseHTTPRequestHandler):
     """SGX HTTP server to complete application config with secrets params."""
 
@@ -38,29 +42,44 @@
         try:
             data = json.loads(body.decode("utf8"))
 
             if app_secrets := data.get("app_secrets"):
                 globs.SECRETS_PATH.parent.mkdir(parents=True, exist_ok=True)
                 globs.SECRETS_PATH.write_bytes(json.dumps(app_secrets).encode("utf-8"))
 
+            if app_sealed_secrets := data.get("app_sealed_secrets"):
+                globs.SEALED_SECRETS_PATH.parent.mkdir(parents=True, exist_ok=True)
+                globs.SEALED_SECRETS_PATH.write_bytes(
+                    json.dumps(
+                        json.loads(
+                            unseal(
+                                base64url_decode(app_sealed_secrets),
+                                globs.ENCLAVE_SK_PATH.read_bytes(),
+                            )
+                        )
+                    ).encode("utf-8")
+                )
+
             # Do not process queries which have not the `uuid` data field
             # Probably a robot
             if data["uuid"] != globs.UUID:
                 self.send_response_only(401)
                 self.end_headers()
                 return
 
             if globs.NEED_SSL_PRIVATE_KEY:
                 globs.SSL_PRIVATE_KEY = data["ssl_private_key"]
 
-            globs.CODE_SECRET_KEY = bytes.fromhex(data["code_secret_key"])
+            if not globs.PLAINCODE:
+                globs.CODE_SECRET_KEY = bytes.fromhex(data["code_secret_key"])
 
-            if len(globs.CODE_SECRET_KEY) != 32:
-                raise CryptoError("Incorrect key length!")
-        except (KeyError, ValueError, json.JSONDecodeError, CryptoError) as exc:
+                if len(globs.CODE_SECRET_KEY) != 32:
+                    raise CryptoError("Incorrect key length!")
+        # might be: KeyError, ValueError, json.JSONDecodeError, CryptoError
+        except Exception as exc:  # pylint: disable=broad-exception-caught
             logging.error(exc)
             self.send_response_only(401)
             self.end_headers()
             return
 
         self.send_response_only(200)
         self.end_headers()
@@ -69,15 +88,15 @@
 
 def serve(
     hostname: str,
     port: int,
     certificate: Certificate,
     uuid: str,
     need_ssl_private_key: bool,
-    timeout: int,
+    timeout: Optional[int],
 ):
     """Serve simple SGX HTTP server."""
     globs.NEED_SSL_PRIVATE_KEY = need_ssl_private_key
     globs.UUID = uuid
 
     httpd = HTTPServer((hostname, port), SGXHTTPRequestHandler)
 
@@ -85,18 +104,19 @@
     ctx.load_cert_chain(
         certfile=str(certificate.cert_path.resolve()),
         keyfile=str(certificate.key_path.resolve()),
     )
 
     httpd.socket = ctx.wrap_socket(httpd.socket, server_side=True)
 
-    timer = threading.Timer(interval=timeout, function=kill)
-    timer.start()
+    if timeout is not None:
+        timer = threading.Timer(interval=timeout, function=kill)
+        timer.start()
 
-    threading.Thread(target=kill_event, args=(httpd, timer)).start()
+        threading.Thread(target=kill_event, args=(httpd, timer)).start()
 
     httpd.serve_forever()
 
 
 def kill_event(httpd: HTTPServer, timer: threading.Timer):
     """Kill HTTP server in a thread if `EXIT_EVENT` is set."""
     while True:
```

### Comparing `mse_lib_sgx-1.1a2/src/mse_lib_sgx/import_hook.py` & `mse_lib_sgx-2.0a1/src/mse_lib_sgx/import_hook.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-1.1a2/src/mse_lib_sgx/sgx_quote.py` & `mse_lib_sgx-2.0a1/src/mse_lib_sgx/sgx/quote.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""mse_lib_sgx.sgx_quote module."""
+"""mse_lib_sgx.sgx.quote module."""
 
 from mse_lib_sgx.error import SGXError
 
 SGX_QUOTE_MAX_SIZE: int = 8192
 
 
 def get_quote(user_report_data: bytes) -> bytes:
```

### Comparing `mse_lib_sgx-1.1a2/src/mse_lib_sgx.egg-info/PKG-INFO` & `mse_lib_sgx-2.0a1/src/mse_lib_sgx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse-lib-sgx
-Version: 1.1a2
+Version: 2.0a1
 Summary: Library for Cosmian MSE to bootstrap Flask application
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -43,35 +43,36 @@
 $ pip install mse-lib-sgx
 ```
 
 ## Usage
 
 ```console
 $ mse-bootstrap --help
-usage: mse-bootstrap [-h] --host HOST --port PORT --app-dir APP_DIR --uuid UUID [--version]
-                     [--debug]
+usage: mse-bootstrap [-h] --host HOST --port PORT --app-dir APP_DIR --uuid
+                     UUID [--version] [--debug]
                      (--self-signed EXPIRATION_DATE | --no-ssl | --certificate CERTIFICATE_PATH)
                      application
 
 Bootstrap ASGI/WSGI Python web application for Gramine
 
 positional arguments:
-  application           Application to dispatch to as path.to.module:instance.path
+  application           ASGI application path (as module:app)
 
 optional arguments:
   -h, --help            show this help message and exit
-  --host HOST           Hostname of the configuration serverIf `--self-signed`, it's also the
-                        hostname of the app server
-  --port PORT           Port of the server
-  --app-dir APP_DIR     Path the microservice application. Read only directory.
-  --uuid UUID           Unique application UUID.
+  --host HOST           hostname of the configuration server, also the
+                        hostname of the app server if `--self-signed`
+  --port PORT           port of the server
+  --app-dir APP_DIR     path of the python web application
+  --uuid UUID           unique application UUID
   --version             show program's version number and exit
-  --debug               Debug mode without SGX
+  --debug               debug mode with more logging
   --self-signed EXPIRATION_DATE
-                        Generate a self-signed certificate for the app. Specify the expiration
-                        date of the certificate as a timestamp since Epoch
-  --no-ssl              Don't use HTTPS connection
+                        generate a self-signed certificate for the web app
+                        with a specific expiration date (Unix time)
+  --no-ssl              use HTTP without SSL
   --certificate CERTIFICATE_PATH
-                        Use the given certificate for the SSL connection. the private key will
-                        be sent using the configuration server
+                        custom certificate used for the SSL connection,
+                        private key must be sent through the configuration
+                        server
 
 ```
```

### Comparing `mse_lib_sgx-1.1a2/src/mse_lib_sgx.egg-info/SOURCES.txt` & `mse_lib_sgx-2.0a1/src/mse_lib_sgx.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 README.md
 setup.cfg
 setup.py
 src/mse_lib_sgx/__init__.py
+src/mse_lib_sgx/base64url.py
 src/mse_lib_sgx/certificate.py
 src/mse_lib_sgx/cli.py
 src/mse_lib_sgx/error.py
 src/mse_lib_sgx/globs.py
 src/mse_lib_sgx/http_server.py
 src/mse_lib_sgx/import_hook.py
-src/mse_lib_sgx/sgx_quote.py
 src/mse_lib_sgx.egg-info/PKG-INFO
 src/mse_lib_sgx.egg-info/SOURCES.txt
 src/mse_lib_sgx.egg-info/dependency_links.txt
 src/mse_lib_sgx.egg-info/entry_points.txt
 src/mse_lib_sgx.egg-info/not-zip-safe
 src/mse_lib_sgx.egg-info/requires.txt
 src/mse_lib_sgx.egg-info/top_level.txt
+src/mse_lib_sgx/sgx/__init__.py
+src/mse_lib_sgx/sgx/key.py
+src/mse_lib_sgx/sgx/quote.py
 tests/test_cert_utils.py
 tests/test_conf_server.py
```

### Comparing `mse_lib_sgx-1.1a2/tests/test_cert_utils.py` & `mse_lib_sgx-2.0a1/tests/test_cert_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from mse_lib_sgx.certificate import to_wildcard_domain
 
 
 def test_wildcard():
     assert to_wildcard_domain("localhost") == "localhost"
+    assert to_wildcard_domain("127.0.0.1") == "127.0.0.1"
     assert to_wildcard_domain("cosmian.app") == "cosmian.app"
     assert to_wildcard_domain(".cosmian.app") == "*.cosmian.app"
     assert (
         to_wildcard_domain("9a5029d5-f769-4749-804e-50f6711bd509.cosmian.app")
         == "*.cosmian.app"
     )
     assert (
```

### Comparing `mse_lib_sgx-1.1a2/tests/test_conf_server.py` & `mse_lib_sgx-2.0a1/tests/test_conf_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import importlib
 import json
-import secrets
 import ssl
 import sys
 import time
 import urllib.request
 
 import pytest
 from mse_lib_crypto.xsalsa20_poly1305 import decrypt_directory
```

