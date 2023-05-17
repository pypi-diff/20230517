# Comparing `tmp/python_x509_pkcs11-0.6.37.tar.gz` & `tmp/python_x509_pkcs11-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_x509_pkcs11-0.6.37.tar", last modified: Thu Mar 30 19:43:42 2023, max compression
+gzip compressed data, was "python_x509_pkcs11-0.7.0.tar", last modified: Wed May 17 13:17:06 2023, max compression
```

## Comparing `python_x509_pkcs11-0.6.37.tar` & `python_x509_pkcs11-0.7.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      812 2023-03-30 17:41:59.524521 python_x509_pkcs11-0.6.37/.github/workflows/centos.yaml
--rw-r--r--   0        0        0      857 2023-03-30 19:38:11.302119 python_x509_pkcs11-0.6.37/.github/workflows/debian.yaml
--rw-r--r--   0        0        0      930 2023-03-30 17:43:58.255523 python_x509_pkcs11-0.6.37/.github/workflows/ubuntu.yaml
--rw-r--r--   0        0        0       73 2023-01-12 22:24:08.716099 python_x509_pkcs11-0.6.37/.gitignore
--rw-r--r--   0        0        0     1045 2023-01-12 22:24:08.716099 python_x509_pkcs11-0.6.37/LICENSE
--rw-r--r--   0        0        0     4284 2023-03-30 17:40:50.103503 python_x509_pkcs11-0.6.37/README.md
--rwxr-xr-x   0        0        0      862 2023-03-30 18:32:21.885561 python_x509_pkcs11-0.6.37/deploy.sh
--rw-r--r--   0        0        0    29171 2023-01-12 22:24:08.718099 python_x509_pkcs11-0.6.37/docs/README.md
--rw-r--r--   0        0        0     1061 2023-03-30 19:38:18.661122 python_x509_pkcs11-0.6.37/pyproject.toml
--rw-r--r--   0        0        0       43 2023-01-12 22:24:08.718099 python_x509_pkcs11-0.6.37/requirements.txt
--rw-r--r--   0        0        0      115 2023-03-30 19:38:23.057123 python_x509_pkcs11-0.6.37/src/python_x509_pkcs11/__init__.py
--rw-r--r--   0        0        0     6686 2023-01-12 22:24:08.719099 python_x509_pkcs11-0.6.37/src/python_x509_pkcs11/ca.py
--rw-r--r--   0        0        0     8143 2023-03-07 05:53:33.212319 python_x509_pkcs11-0.6.37/src/python_x509_pkcs11/crl.py
--rw-r--r--   0        0        0     6437 2023-03-30 18:47:00.980330 python_x509_pkcs11-0.6.37/src/python_x509_pkcs11/crypto.py
--rw-r--r--   0        0        0     8805 2023-03-30 18:33:41.270535 python_x509_pkcs11-0.6.37/src/python_x509_pkcs11/csr.py
--rw-r--r--   0        0        0      802 2023-01-12 22:24:08.720099 python_x509_pkcs11-0.6.37/src/python_x509_pkcs11/error.py
--rw-r--r--   0        0        0     1889 2023-01-12 22:24:08.720099 python_x509_pkcs11-0.6.37/src/python_x509_pkcs11/lib.py
--rw-r--r--   0        0        0    13591 2023-03-30 18:35:32.688507 python_x509_pkcs11-0.6.37/src/python_x509_pkcs11/ocsp.py
--rw-r--r--   0        0        0    20073 2023-03-30 19:14:12.608687 python_x509_pkcs11-0.6.37/src/python_x509_pkcs11/pkcs11_handle.py
--rw-r--r--   0        0        0        0 2023-01-12 22:24:08.722099 python_x509_pkcs11-0.6.37/src/python_x509_pkcs11/py.typed
--rw-r--r--   0        0        0        0 2023-01-12 22:24:08.722099 python_x509_pkcs11-0.6.37/tests/__init__.py
--rw-r--r--   0        0        0    14068 2023-03-30 18:20:15.397694 python_x509_pkcs11-0.6.37/tests/test_ca.py
--rw-r--r--   0        0        0     9646 2023-03-07 06:02:21.968258 python_x509_pkcs11-0.6.37/tests/test_crl.py
--rw-r--r--   0        0        0     4049 2023-01-12 22:24:08.723099 python_x509_pkcs11-0.6.37/tests/test_crypto.py
--rw-r--r--   0        0        0    11078 2023-01-12 22:24:08.723099 python_x509_pkcs11-0.6.37/tests/test_csr.py
--rw-r--r--   0        0        0    33955 2023-03-30 17:29:42.252213 python_x509_pkcs11-0.6.37/tests/test_ocsp.py
--rw-r--r--   0        0        0    43289 2023-02-28 20:00:22.793094 python_x509_pkcs11-0.6.37/tests/test_pkcs11_handle.py
--rw-r--r--   0        0        0     4722 1970-01-01 00:00:00.000000 python_x509_pkcs11-0.6.37/PKG-INFO
+-rw-r--r--   0        0        0      812 2023-03-30 17:41:59.524521 python_x509_pkcs11-0.7.0/.github/workflows/centos.yaml
+-rw-r--r--   0        0        0      857 2023-03-30 19:38:11.302119 python_x509_pkcs11-0.7.0/.github/workflows/debian.yaml
+-rw-r--r--   0        0        0      930 2023-03-30 17:43:58.255523 python_x509_pkcs11-0.7.0/.github/workflows/ubuntu.yaml
+-rw-r--r--   0        0        0       73 2023-01-12 22:24:08.716099 python_x509_pkcs11-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1045 2023-01-12 22:24:08.716099 python_x509_pkcs11-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4284 2023-03-30 17:40:50.103503 python_x509_pkcs11-0.7.0/README.md
+-rwxr-xr-x   0        0        0      862 2023-03-30 18:32:21.885561 python_x509_pkcs11-0.7.0/deploy.sh
+-rw-r--r--   0        0        0    29171 2023-01-12 22:24:08.718099 python_x509_pkcs11-0.7.0/docs/README.md
+-rw-r--r--   0        0        0     1084 2023-05-17 13:00:48.485780 python_x509_pkcs11-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-01-12 22:24:08.718099 python_x509_pkcs11-0.7.0/requirements.txt
+-rw-r--r--   0        0        0      114 2023-05-17 13:00:48.490780 python_x509_pkcs11-0.7.0/src/python_x509_pkcs11/__init__.py
+-rw-r--r--   0        0        0     6686 2023-01-12 22:24:08.719099 python_x509_pkcs11-0.7.0/src/python_x509_pkcs11/ca.py
+-rw-r--r--   0        0        0     8143 2023-03-07 05:53:33.212319 python_x509_pkcs11-0.7.0/src/python_x509_pkcs11/crl.py
+-rw-r--r--   0        0        0     6437 2023-03-30 18:47:00.980330 python_x509_pkcs11-0.7.0/src/python_x509_pkcs11/crypto.py
+-rw-r--r--   0        0        0     8805 2023-03-30 18:33:41.270535 python_x509_pkcs11-0.7.0/src/python_x509_pkcs11/csr.py
+-rw-r--r--   0        0        0      802 2023-01-12 22:24:08.720099 python_x509_pkcs11-0.7.0/src/python_x509_pkcs11/error.py
+-rw-r--r--   0        0        0     1889 2023-01-12 22:24:08.720099 python_x509_pkcs11-0.7.0/src/python_x509_pkcs11/lib.py
+-rw-r--r--   0        0        0    13591 2023-03-30 18:35:32.688507 python_x509_pkcs11-0.7.0/src/python_x509_pkcs11/ocsp.py
+-rw-r--r--   0        0        0    23077 2023-05-17 13:12:47.178470 python_x509_pkcs11-0.7.0/src/python_x509_pkcs11/pkcs11_handle.py
+-rw-r--r--   0        0        0        0 2023-01-12 22:24:08.722099 python_x509_pkcs11-0.7.0/src/python_x509_pkcs11/py.typed
+-rw-r--r--   0        0        0        0 2023-01-12 22:24:08.722099 python_x509_pkcs11-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0    14068 2023-03-30 18:20:15.397694 python_x509_pkcs11-0.7.0/tests/test_ca.py
+-rw-r--r--   0        0        0     9646 2023-03-07 06:02:21.968258 python_x509_pkcs11-0.7.0/tests/test_crl.py
+-rw-r--r--   0        0        0     4049 2023-01-12 22:24:08.723099 python_x509_pkcs11-0.7.0/tests/test_crypto.py
+-rw-r--r--   0        0        0    11078 2023-01-12 22:24:08.723099 python_x509_pkcs11-0.7.0/tests/test_csr.py
+-rw-r--r--   0        0        0    33955 2023-03-30 17:29:42.252213 python_x509_pkcs11-0.7.0/tests/test_ocsp.py
+-rw-r--r--   0        0        0    45391 2023-05-17 13:15:40.924922 python_x509_pkcs11-0.7.0/tests/test_pkcs11_handle.py
+-rw-r--r--   0        0        0     4721 1970-01-01 00:00:00.000000 python_x509_pkcs11-0.7.0/PKG-INFO
```

### Comparing `python_x509_pkcs11-0.6.37/.github/workflows/centos.yaml` & `python_x509_pkcs11-0.7.0/.github/workflows/centos.yaml`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.6.37/.github/workflows/debian.yaml` & `python_x509_pkcs11-0.7.0/.github/workflows/debian.yaml`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.6.37/.github/workflows/ubuntu.yaml` & `python_x509_pkcs11-0.7.0/.github/workflows/ubuntu.yaml`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.6.37/LICENSE` & `python_x509_pkcs11-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.6.37/README.md` & `python_x509_pkcs11-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.6.37/deploy.sh` & `python_x509_pkcs11-0.7.0/deploy.sh`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.6.37/docs/README.md` & `python_x509_pkcs11-0.7.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.6.37/pyproject.toml` & `python_x509_pkcs11-0.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 description = "Python async library for signing x509 using keys in an pkcs11 device such as a HSM"
-version = "0.6.37"
+version = "0.7.0"
 
 [build-system]
 requires = [
     "flit_core >=2.0",
 ]
 
 [tool.flit.metadata]
@@ -38,14 +38,15 @@
     "asn1crypto.core",
     "asn1crypto.x509",
     "asn1crypto.csr",
     "asn1crypto.crl",
     "pkcs11",
     "pkcs11.util.ec",
     "pkcs11.util.rsa",
+    "pkcs11.util.x509",
     "pkcs11.exceptions",
 ]
 ignore_missing_imports = true
 
 [tool.isort]
 profile = "black"
 src_paths = ["src", "tests"]
```

### Comparing `python_x509_pkcs11-0.6.37/src/python_x509_pkcs11/ca.py` & `python_x509_pkcs11-0.7.0/src/python_x509_pkcs11/ca.py`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.6.37/src/python_x509_pkcs11/crl.py` & `python_x509_pkcs11-0.7.0/src/python_x509_pkcs11/crl.py`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.6.37/src/python_x509_pkcs11/crypto.py` & `python_x509_pkcs11-0.7.0/src/python_x509_pkcs11/crypto.py`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.6.37/src/python_x509_pkcs11/csr.py` & `python_x509_pkcs11-0.7.0/src/python_x509_pkcs11/csr.py`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.6.37/src/python_x509_pkcs11/error.py` & `python_x509_pkcs11-0.7.0/src/python_x509_pkcs11/error.py`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.6.37/src/python_x509_pkcs11/lib.py` & `python_x509_pkcs11-0.7.0/src/python_x509_pkcs11/lib.py`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.6.37/src/python_x509_pkcs11/ocsp.py` & `python_x509_pkcs11-0.7.0/src/python_x509_pkcs11/ocsp.py`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.6.37/src/python_x509_pkcs11/pkcs11_handle.py` & `python_x509_pkcs11-0.7.0/src/python_x509_pkcs11/pkcs11_handle.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Module which handles a PKCS11 session and its exposed methods
 
 # Better to keep a pkcs11 session reference all the time
 # and then when it fails to open a new session for performance
 # See PKCS11Session._healthy_session()
 
 Exposes the functions:
+- import_certificate()
+- export_certificate()
+- delete_certificate()
 - import_keypair()
 - create_keypair()
 - key_labels()
 - sign()
 - verify()
 - delete_keypair()
 - public_key_data()
@@ -19,14 +22,15 @@
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import asynccontextmanager
 from hashlib import sha256, sha384, sha512
 from threading import Lock, Thread
 from typing import AsyncIterator, Dict, Optional, Tuple
 
 from asn1crypto import pem as asn1_pem
+from asn1crypto import x509 as asn1_x509
 from asn1crypto.algos import SignedDigestAlgorithmId
 from asn1crypto.keys import (
     PublicKeyAlgorithm,
     PublicKeyAlgorithmId,
     PublicKeyInfo,
     RSAPublicKey,
 )
@@ -44,14 +48,15 @@
     encode_named_curve_parameters,
 )
 from pkcs11.util.rsa import (
     decode_rsa_private_key,
     decode_rsa_public_key,
     encode_rsa_public_key,
 )
+from pkcs11.util.x509 import decode_x509_certificate
 
 from .crypto import (
     convert_asn1_ec_signature,
     convert_rs_ec_signature,
     decode_eddsa_private_key,
     decode_eddsa_public_key,
     encode_eddsa_public_key,
@@ -178,14 +183,100 @@
             await sleep(0)
             thread2.join(timeout=TIMEOUT)
 
             if thread2.is_alive() or cls._session_status != 0:
                 raise PKCS11UnknownErrorException("ERROR: Could not get a healthy PKCS11 connection in time")
 
     @classmethod
+    async def import_certificate(cls, cert_pem: str, cert_label: str) -> None:
+        """Import a certificate into the PKCS11 device with this label.
+
+        Parameters:
+        cert_pem (str): Certificate in PEM form.
+        cert_label (str): Certificate label in the PKCS11 device.
+
+        Returns:
+        None
+        """
+
+        async with async_lock(cls.lock):
+            # Ensure we get a healthy pkcs11 session
+            await cls.healthy_session()
+
+            for cert in cls.session.get_objects(
+                {
+                    Attribute.CLASS: ObjectClass.CERTIFICATE,
+                    Attribute.LABEL: cert_label,
+                }
+            ):
+                raise ValueError("Certificate with that label already exists in the PKCS11 device")
+
+            data = cert_pem.encode("utf-8")
+            if asn1_pem.detect(data):
+                _, _, data = asn1_pem.unarmor(data)
+
+            cert = decode_x509_certificate(data)
+            cert[Attribute.TOKEN] = True
+            cert[Attribute.LABEL] = cert_label
+            cls.session.create_object(cert)
+
+    @classmethod
+    async def export_certificate(cls, cert_label: str) -> str:
+        """Export a certificate from the PKCS11 device with this label.
+        Returns the PEM encoded cert.
+
+        Parameters:
+        cert_label (str): Certificate label in the PKCS11 device.
+
+        Returns:
+        str
+        """
+
+        async with async_lock(cls.lock):
+            # Ensure we get a healthy pkcs11 session
+            await cls.healthy_session()
+
+            for cert in cls.session.get_objects(
+                {
+                    Attribute.CLASS: ObjectClass.CERTIFICATE,
+                    Attribute.LABEL: cert_label,
+                }
+            ):
+                der_bytes = cert[Attribute.VALUE]
+
+                # Load a certificate object from the DER-encoded value
+                cert_asn1 = asn1_x509.Certificate.load(der_bytes)
+
+                # Write out a PEM encoded value
+                ret: bytes = asn1_pem.armor("CERTIFICATE", cert_asn1.dump())
+                return ret.decode("utf-8")
+
+            raise ValueError("No such certificate in the PKCS11 device")
+
+    @classmethod
+    async def delete_certificate(cls, cert_label: str) -> None:
+        """Delete a certificate from the PKCS11 device with this label.
+
+        Parameters:
+        cert_label (str): Certificate label in the PKCS11 device.
+        """
+
+        async with async_lock(cls.lock):
+            # Ensure we get a healthy pkcs11 session
+            await cls.healthy_session()
+
+            for cert in cls.session.get_objects(
+                {
+                    Attribute.CLASS: ObjectClass.CERTIFICATE,
+                    Attribute.LABEL: cert_label,
+                }
+            ):
+                cert.destroy()
+
+    @classmethod
     async def import_keypair(cls, public_key: bytes, private_key: bytes, key_label: str, key_type: str) -> None:
         """Import a DER encoded keypair into the PKCS11 device with this label.
         If the label already exists in the PKCS11 device then raise pkcs11.MultipleObjectsReturned.
 
         Generating public_key and private_key can be done with:
         openssl genpkey -algorithm ed25519 -out private.pem
         openssl pkey -in private.pem -outform DER -out private.key
```

### Comparing `python_x509_pkcs11-0.6.37/tests/test_ca.py` & `python_x509_pkcs11-0.7.0/tests/test_ca.py`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.6.37/tests/test_crl.py` & `python_x509_pkcs11-0.7.0/tests/test_crl.py`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.6.37/tests/test_crypto.py` & `python_x509_pkcs11-0.7.0/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.6.37/tests/test_csr.py` & `python_x509_pkcs11-0.7.0/tests/test_csr.py`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.6.37/tests/test_ocsp.py` & `python_x509_pkcs11-0.7.0/tests/test_ocsp.py`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.6.37/tests/test_pkcs11_handle.py` & `python_x509_pkcs11-0.7.0/tests/test_pkcs11_handle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Test our PKCS11 session handler
 """
 import asyncio
 import os
 import unittest
 
+# import asn1crypto.x509 as asn1_x509
 from pkcs11.exceptions import MultipleObjectsReturned, NoSuchKey
 
 from src.python_x509_pkcs11.error import PKCS11UnknownErrorException
 from src.python_x509_pkcs11.lib import key_types
 from src.python_x509_pkcs11.pkcs11_handle import PKCS11Session
 
 # Replace the above with this should you use this code
@@ -544,7 +545,49 @@
                     key_type="rsa_2048",
                 )
             )
         )
 
         # Delete the test key
         asyncio.run(PKCS11Session.delete_keypair(new_key_label, key_type="rsa_2048"))
+
+    def test_import_export_delete_cert(self) -> None:
+        """
+        Import, export and delete cert to and from the PKCS11 device.
+        """
+
+        cert_pem = """-----BEGIN CERTIFICATE-----
+MIIDYzCCAkugAwIBAgIUN+IOJqkvZDa5clXCnrZi+jFxoG4wDQYJKoZIhvcNAQEL
+BQAwQTELMAkGA1UEBhMCU0UxEjAQBgNVBAcMCVN0b2NraG9sbTEOMAwGA1UECgwF
+U1VORVQxDjAMBgNVBAMMBVNVTkVUMB4XDTIzMDUwNTA5MTIyMFoXDTI0MDUwNDA5
+MTIyMFowQTELMAkGA1UEBhMCU0UxEjAQBgNVBAcMCVN0b2NraG9sbTEOMAwGA1UE
+CgwFU1VORVQxDjAMBgNVBAMMBVNVTkVUMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8A
+MIIBCgKCAQEA+NZi3Ipp67cEf5M8A7Lr94vS4Cg74huGymEfuAGbF5TiUuusOUJd
+mdVfKrKLL8zHK42tyUfhTx0tBUrHWIu3/aeEtGEYh5VgmLk2y/K8p09cUTd4l5SA
+hzIf76PC7Ux0rCIZ3IFbHQ/eWLoAxvjAIMMZd4+Rby3iCw7Ula6ruEIBoLWpBn+c
+NOpq4XvOsudSz8VJuLYP6gAbJLo2V+BXQaC5R/HUtEeuS4iC66LfrwEG7Aj/n/9o
+OIUmSZby5LFnPz/D2YbIsozWJkFIt8Z2PZRngQrQ1K3LfuVkfbVlRUSlFrQhgFg4
+yKsGLm3eByZR6o28EdAU0wIZTrbSBmCyKwIDAQABo1MwUTAdBgNVHQ4EFgQU69PY
+JB3mcLLsDKjzi/esyq4X/UYwHwYDVR0jBBgwFoAU69PYJB3mcLLsDKjzi/esyq4X
+/UYwDwYDVR0TAQH/BAUwAwEB/zANBgkqhkiG9w0BAQsFAAOCAQEAryGICswCRVeO
+lotVftUXIPRUVDFwvovfpQi407GfchWW6qfi8QMtD8SP/I+lySTUFE1Tm9gb7OHT
+3FPtYatzsqUQN0W2sf9EDjkQDHuMKGtBi7ZWYpKUllyCdBUKEukWNKPeVUwOYxOW
+mV72a3xICxRafOrsOyfYY/3xpdocJynYr5TBvXDWDmGRKz+9vlUUCazHMlLxxK9W
+owuSqWzudPixJNEFnjUXloAafbP1NU+HnVOG2daJqyVpSaiCTyjsK1iJ6hWWMu+g
+Z0C3qdoke9EvHCcwjbvJ8U5Bq5obD8D7nxSKIt/eEjSpqfhdOU3xC98uFxl6709v
+tnmQdMO1DA==
+-----END CERTIFICATE-----
+"""
+
+        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        asyncio.run(PKCS11Session.import_certificate(cert_pem, new_key_label))
+        with self.assertRaises(ValueError):
+            asyncio.run(PKCS11Session.import_certificate(cert_pem, new_key_label))
+
+        cert = asyncio.run(PKCS11Session.export_certificate(new_key_label))
+
+        self.assertTrue(isinstance(cert, str) and len(cert) > 0)
+        self.assertTrue(cert_pem == cert)
+
+        asyncio.run(PKCS11Session.delete_certificate(new_key_label))
+        with self.assertRaises(ValueError):
+            asyncio.run(PKCS11Session.export_certificate(new_key_label))
```

### Comparing `python_x509_pkcs11-0.6.37/PKG-INFO` & `python_x509_pkcs11-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_x509_pkcs11
-Version: 0.6.37
+Version: 0.7.0
 Summary: Python async library for signing x509 using keys in a pkcs11 device such as an HSM.
 Home-page: https://github.com/SUNET/python_x509_pkcs11
 License: MIT
 Keywords: x509,pkcs11,HSM
 Author: Victor Näslund
 Author-email: victor@sunet.se
 Requires-Python: >=3.8
```

