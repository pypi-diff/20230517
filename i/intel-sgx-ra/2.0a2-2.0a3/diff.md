# Comparing `tmp/intel_sgx_ra-2.0a2.tar.gz` & `tmp/intel_sgx_ra-2.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intel_sgx_ra-2.0a2.tar", last modified: Wed May 10 15:25:55 2023, max compression
+gzip compressed data, was "intel_sgx_ra-2.0a3.tar", last modified: Wed May 17 13:01:32 2023, max compression
```

## Comparing `intel_sgx_ra-2.0a2.tar` & `intel_sgx_ra-2.0a3.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:25:55.398874 intel_sgx_ra-2.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-10 15:25:55.398874 intel_sgx_ra-2.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-10 15:25:13.000000 intel_sgx_ra-2.0a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-10 15:25:55.398874 intel_sgx_ra-2.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-10 15:25:13.000000 intel_sgx_ra-2.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:25:55.394874 intel_sgx_ra-2.0a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:25:55.398874 intel_sgx_ra-2.0a2/src/intel_sgx_ra/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-10 15:25:13.000000 intel_sgx_ra-2.0a2/src/intel_sgx_ra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-05-10 15:25:13.000000 intel_sgx_ra-2.0a2/src/intel_sgx_ra/attest.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-10 15:25:13.000000 intel_sgx_ra-2.0a2/src/intel_sgx_ra/base64url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:25:55.398874 intel_sgx_ra-2.0a2/src/intel_sgx_ra/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-10 15:25:13.000000 intel_sgx_ra-2.0a2/src/intel_sgx_ra/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-10 15:25:13.000000 intel_sgx_ra-2.0a2/src/intel_sgx_ra/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-10 15:25:13.000000 intel_sgx_ra-2.0a2/src/intel_sgx_ra/cli/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-10 15:25:13.000000 intel_sgx_ra-2.0a2/src/intel_sgx_ra/error.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-10 15:25:13.000000 intel_sgx_ra-2.0a2/src/intel_sgx_ra/globs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-10 15:25:13.000000 intel_sgx_ra-2.0a2/src/intel_sgx_ra/pccs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:25:13.000000 intel_sgx_ra-2.0a2/src/intel_sgx_ra/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-05-10 15:25:13.000000 intel_sgx_ra-2.0a2/src/intel_sgx_ra/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-10 15:25:13.000000 intel_sgx_ra-2.0a2/src/intel_sgx_ra/ratls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-10 15:25:13.000000 intel_sgx_ra-2.0a2/src/intel_sgx_ra/signer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:25:55.398874 intel_sgx_ra-2.0a2/src/intel_sgx_ra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-10 15:25:55.000000 intel_sgx_ra-2.0a2/src/intel_sgx_ra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-10 15:25:55.000000 intel_sgx_ra-2.0a2/src/intel_sgx_ra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:25:55.000000 intel_sgx_ra-2.0a2/src/intel_sgx_ra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-10 15:25:55.000000 intel_sgx_ra-2.0a2/src/intel_sgx_ra.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:25:55.000000 intel_sgx_ra-2.0a2/src/intel_sgx_ra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 15:25:55.000000 intel_sgx_ra-2.0a2/src/intel_sgx_ra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 15:25:55.000000 intel_sgx_ra-2.0a2/src/intel_sgx_ra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:25:55.398874 intel_sgx_ra-2.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-10 15:25:13.000000 intel_sgx_ra-2.0a2/tests/test_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-10 15:25:13.000000 intel_sgx_ra-2.0a2/tests/test_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:32.751222 intel_sgx_ra-2.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-17 13:01:32.751222 intel_sgx_ra-2.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-17 13:01:32.751222 intel_sgx_ra-2.0a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:32.743221 intel_sgx_ra-2.0a3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:32.747221 intel_sgx_ra-2.0a3/src/intel_sgx_ra/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/attest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/base64url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:32.747221 intel_sgx_ra-2.0a3/src/intel_sgx_ra/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/cli/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/globs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/pccs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/ratls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/signer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:32.747221 intel_sgx_ra-2.0a3/src/intel_sgx_ra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-17 13:01:32.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-17 13:01:32.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:01:32.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-17 13:01:32.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:01:32.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-17 13:01:32.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 13:01:32.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:32.751222 intel_sgx_ra-2.0a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/tests/test_pccs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/tests/test_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/tests/test_regex.py
```

### Comparing `intel_sgx_ra-2.0a2/PKG-INFO` & `intel_sgx_ra-2.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intel_sgx_ra
-Version: 2.0a2
+Version: 2.0a3
 Summary: Intel SGX Remote Attestation verification library
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `intel_sgx_ra-2.0a2/README.md` & `intel_sgx_ra-2.0a3/README.md`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a2/setup.py` & `intel_sgx_ra-2.0a3/setup.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a2/src/intel_sgx_ra/attest.py` & `intel_sgx_ra-2.0a3/src/intel_sgx_ra/attest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,125 +1,178 @@
 """intel_ra_sgx.attest module."""
 
 import logging
+from datetime import datetime
+from hashlib import sha256
 from typing import Union, cast
 
 import cryptography.exceptions
 from cryptography import x509
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.hazmat.primitives.asymmetric.utils import encode_dss_signature
 from cryptography.hazmat.primitives.hashes import SHA256, HashAlgorithm
 
 from intel_sgx_ra import globs
-from intel_sgx_ra.error import CertificateRevokedError, SGXDebugModeError
+from intel_sgx_ra.error import (
+    CertificateError,
+    CertificateRevokedError,
+    SGXDebugModeError,
+    SGXVerificationError,
+)
 from intel_sgx_ra.pccs import get_pck_cert_crl, get_root_ca_crl
 from intel_sgx_ra.quote import Quote
 
 # define SGX_FLAGS_DEBUG 0x0000000000000002ULL
 SGX_FLAGS_DEBUG: int = 2
 
 
-def verify_quote(quote: Union[Quote, bytes], base_url: str):
-    """Process DCAP remote attestation with `quote`."""
-    quote = cast(Quote, Quote.from_bytes(quote) if isinstance(quote, bytes) else quote)
-
-    # If set, then the enclave is in debug mode
-    debug: bool = bool(quote.report_body.flags & SGX_FLAGS_DEBUG)
-
-    logging.info("%s No SGX debug mode", globs.FAIL if debug else globs.OK)
-
-    if debug:
-        raise SGXDebugModeError
+def verify_pck_chain(
+    root_ca_cert: x509.Certificate,
+    pck_ca_cert: x509.Certificate,
+    pck_cert: x509.Certificate,
+    root_ca_crl: x509.CertificateRevocationList,
+    pck_ca_crl: x509.CertificateRevocationList,
+) -> bool:
+    """PCK certification chain validation."""
+    now: datetime = datetime.utcnow()
 
-    pck_cert, pck_platform_ca_cert, root_ca_cert = [
-        x509.load_pem_x509_certificate(raw_cert) for raw_cert in quote.certs()
-    ]  # type: x509.Certificate, x509.Certificate, x509.Certificate
-    pck_pk, pck_platform_ca_pk, root_ca_pk = (
-        cast(ec.EllipticCurvePublicKey, pck_cert.public_key()),
-        cast(ec.EllipticCurvePublicKey, pck_platform_ca_cert.public_key()),
+    pck_ca_pk, root_ca_pk = (
+        cast(ec.EllipticCurvePublicKey, pck_ca_cert.public_key()),
         cast(ec.EllipticCurvePublicKey, root_ca_cert.public_key()),
     )
 
-    root_ca_crl: x509.CertificateRevocationList = get_root_ca_crl(base_url)
-    # Check that Intel Root CA signed Intel Root CA CRL
-    assert root_ca_crl.is_signature_valid(root_ca_pk)
+    # Check issuers
+    root_ca_cert.verify_directly_issued_by(root_ca_cert)
+    pck_ca_cert.verify_directly_issued_by(root_ca_cert)
+    pck_cert.verify_directly_issued_by(pck_ca_cert)
+
+    # Check expiration date of certificates
+    if not root_ca_cert.not_valid_before <= now <= root_ca_cert.not_valid_after:
+        raise CertificateError("Intel Root CA certificate has expired")
+    if not pck_ca_cert.not_valid_before <= now <= pck_ca_cert.not_valid_after:
+        raise CertificateError("Intel PCK CA certificate has expired")
+    if not pck_cert.not_valid_before <= now <= pck_cert.not_valid_after:
+        raise CertificateError("Intel PCK certificate has expired")
+
+    # Check Intel Root CA signed Intel Root CA CRL and not revoked
+    if not root_ca_crl.is_signature_valid(root_ca_pk):
+        raise CertificateError("Invalid Intel Root CA CRL signature")
+
     if root_ca_crl.get_revoked_certificate_by_serial_number(root_ca_cert.serial_number):
         logging.info("%s Check Intel Root CA certificate against CRL", globs.FAIL)
         raise CertificateRevokedError("Intel Root CA certificate revoked")
 
-    pck_platform_crl = get_pck_cert_crl(base_url, "platform")
-    # Check that Intel PCK Platform signed Intel PCK CRL
-    assert pck_platform_crl.is_signature_valid(pck_platform_ca_pk)
-    if pck_platform_crl.get_revoked_certificate_by_serial_number(
-        pck_platform_ca_cert.serial_number
-    ):
-        logging.info("%s Check Intel PCK Platform certificate against CRL", globs.FAIL)
-        raise CertificateRevokedError("Intel PCK Platform certificate revoked")
-
-    logging.info("%s Check Certificate Revocation List (CRL)", globs.OK)
+    # Check Intel PCK Platform/Processor signed Intel PCK CRL and not revoked
+    if not pck_ca_crl.is_signature_valid(pck_ca_pk):
+        raise CertificateError("Invalid Intel PCK CA CRL signature")
+
+    if pck_ca_crl.get_revoked_certificate_by_serial_number(pck_ca_cert.serial_number):
+        logging.info("%s Check Intel PCK CA certificate against CRL", globs.FAIL)
+        raise CertificateRevokedError("Intel PCK CA certificate revoked")
 
     try:
         # 1) Check Intel Root CA is self-signed
         root_ca_pk.verify(
             root_ca_cert.signature,
             root_ca_cert.tbs_certificate_bytes,
             ec.ECDSA(cast(HashAlgorithm, root_ca_cert.signature_hash_algorithm)),
         )
-        # 2) Check Intel Root CA signed Intel PCK Platform CA
+        # 2) Check Intel Root CA signed Intel PCK Platform/Processor CA
         root_ca_pk.verify(
-            pck_platform_ca_cert.signature,
-            pck_platform_ca_cert.tbs_certificate_bytes,
-            ec.ECDSA(
-                cast(HashAlgorithm, pck_platform_ca_cert.signature_hash_algorithm)
-            ),
+            pck_ca_cert.signature,
+            pck_ca_cert.tbs_certificate_bytes,
+            ec.ECDSA(cast(HashAlgorithm, pck_ca_cert.signature_hash_algorithm)),
         )
-        # 3) Check Intel PCK Platform CA signed Intel PCK certificate
-        pck_platform_ca_pk.verify(
+        # 3) Check Intel PCK Platform/Processor CA signed Intel PCK certificate
+        pck_ca_pk.verify(
             pck_cert.signature,
             pck_cert.tbs_certificate_bytes,
             ec.ECDSA(cast(HashAlgorithm, pck_cert.signature_hash_algorithm)),
         )
     except cryptography.exceptions.InvalidSignature as exc:
         logging.info("%s Certification chain", globs.FAIL)
         raise exc
 
     logging.info("%s Certification chain", globs.OK)
 
-    pk = ec.EllipticCurvePublicNumbers(
+    return True
+
+
+def verify_quote(quote: Union[Quote, bytes], pccs_url: str):
+    """Process DCAP remote attestation with `quote`."""
+    quote = cast(Quote, Quote.from_bytes(quote) if isinstance(quote, bytes) else quote)
+
+    # If set, then the enclave is in debug mode
+    debug: bool = bool(quote.report_body.flags & SGX_FLAGS_DEBUG)
+
+    logging.info("%s No SGX debug mode", globs.FAIL if debug else globs.OK)
+
+    if debug:
+        raise SGXDebugModeError
+
+    pck_cert, pck_ca_cert, root_ca_cert = [
+        x509.load_pem_x509_certificate(raw_cert) for raw_cert in quote.certs()
+    ]  # type: x509.Certificate, x509.Certificate, x509.Certificate
+
+    root_ca_crl: x509.CertificateRevocationList = get_root_ca_crl(pccs_url)
+    common_name, *_ = pck_ca_cert.subject.get_attributes_for_oid(
+        x509.NameOID.COMMON_NAME
+    )
+    pck_ca_crl: x509.CertificateRevocationList
+    if common_name.value == "Intel SGX PCK Platform CA":
+        pck_ca_crl = get_pck_cert_crl(pccs_url, "platform")
+    elif common_name.value == "Intel SGX PCK Processor CA":
+        pck_ca_crl = get_pck_cert_crl(pccs_url, "processor")
+    else:
+        raise CertificateError("Unknown CN in Intel SGX PCK Platform/Processor CA")
+
+    assert verify_pck_chain(
+        root_ca_cert, pck_ca_cert, pck_cert, root_ca_crl, pck_ca_crl
+    )
+
+    ecdsa_attestation_pk = ec.EllipticCurvePublicNumbers(
         curve=ec.SECP256R1(),
         x=int.from_bytes(quote.auth_data.public_key[:32], byteorder="big"),
         y=int.from_bytes(quote.auth_data.public_key[32:], byteorder="big"),
     ).public_key()
 
     try:
-        pk.verify(
+        ecdsa_attestation_pk.verify(
             signature=encode_dss_signature(
                 r=int.from_bytes(quote.auth_data.signature[:32], byteorder="big"),
                 s=int.from_bytes(quote.auth_data.signature[32:], byteorder="big"),
             ),
             data=bytes(quote.header) + bytes(quote.report_body),
             signature_algorithm=ec.ECDSA(SHA256()),
         )
     except cryptography.exceptions.InvalidSignature as exc:
         logging.info("%s Quote signature", globs.FAIL)
         raise exc
 
     logging.info("%s Quote signature", globs.OK)
 
     try:
+        pck_pk = cast(ec.EllipticCurvePublicKey, pck_cert.public_key())
         pck_pk.verify(
             signature=encode_dss_signature(
                 r=int.from_bytes(
                     quote.auth_data.qe_report_signature[:32], byteorder="big"
                 ),
                 s=int.from_bytes(
                     quote.auth_data.qe_report_signature[32:], byteorder="big"
                 ),
             ),
-            data=quote.auth_data.qe_report,
+            data=bytes(quote.auth_data.qe_report),
             signature_algorithm=ec.ECDSA(SHA256()),
         )
     except cryptography.exceptions.InvalidSignature as exc:
         logging.info("%s QE report signature", globs.FAIL)
         raise exc
 
+    expected_qe_report_data: bytes = sha256(
+        quote.auth_data.public_key + quote.auth_data.qe_auth_data
+    ).digest()
+
+    if quote.auth_data.qe_report.report_data[:32] != expected_qe_report_data:
+        raise SGXVerificationError("Unexpected REPORTDATA in QE report")
+
     logging.info("%s QE report signature", globs.OK)
```

### Comparing `intel_sgx_ra-2.0a2/src/intel_sgx_ra/base64url.py` & `intel_sgx_ra-2.0a3/src/intel_sgx_ra/base64url.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a2/src/intel_sgx_ra/cli/utils.py` & `intel_sgx_ra-2.0a3/src/intel_sgx_ra/cli/utils.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a2/src/intel_sgx_ra/cli/verify.py` & `intel_sgx_ra-2.0a3/src/intel_sgx_ra/cli/verify.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 import logging
 import os
 import sys
 import traceback
 from pathlib import Path
 from pprint import pformat
 
+from intel_sgx_ra import globs
 from intel_sgx_ra.attest import verify_quote
 from intel_sgx_ra.error import (
     CertificateRevokedError,
     CommandNotFound,
     RATLSVerificationError,
     SGXDebugModeError,
     SGXQuoteNotFound,
 )
 from intel_sgx_ra.quote import Quote
 from intel_sgx_ra.ratls import ratls_verify, ratls_verify_from_url
 
-BASE_URL: str = os.getenv("PCCS_URL", "https://pccs.mse.cosmian.com")
+PCCS_URL: str = os.getenv("PCCS_URL", "https://pccs.mse.cosmian.com")
 
 
 def parse_args() -> argparse.Namespace:
     """CLI argument parser."""
     parser = argparse.ArgumentParser(description="Intel SGX DCAP Quote verification")
     parser.add_argument("--verbose", action="store_true", help="Verbose mode")
     parser.add_argument(
@@ -70,15 +71,15 @@
         )
     elif args.command == "quote":
         quote = Quote.from_bytes(args.path.resolve().read_bytes())
     else:
         raise CommandNotFound("Bad subcommand!")
 
     try:
-        verify_quote(quote=quote, base_url=BASE_URL)
+        verify_quote(quote=quote, pccs_url=PCCS_URL)
     except SGXQuoteNotFound:
         traceback.print_exc()
         sys.exit(1)
     except RATLSVerificationError:
         traceback.print_exc()
         sys.exit(2)
     except SGXDebugModeError:
@@ -86,23 +87,23 @@
         sys.exit(3)
     except CertificateRevokedError:
         traceback.print_exc()
         sys.exit(4)
 
     if args.mrenclave:
         if quote.report_body.mr_enclave == bytes.fromhex(args.mrenclave):
-            logging.info("[   OK ] MRENCLAVE matches expected value")
+            logging.info("%s MRENCLAVE matches expected value", globs.OK)
         else:
-            logging.info("[ FAIL ] MRENCLAVE matches expected value")
+            logging.info("%s MRENCLAVE matches expected value", globs.FAIL)
             sys.exit(5)
 
     if args.mrsigner:
         if quote.report_body.mr_signer == bytes.fromhex(args.mrsigner):
-            logging.info("[   OK ] MRSIGNER matches expected value")
+            logging.info("%s MRSIGNER matches expected value", globs.OK)
         else:
-            logging.info("[ FAIL ] MRSIGNER matches expected value")
+            logging.info("%s MRSIGNER matches expected value", globs.FAIL)
             sys.exit(6)
 
     if args.verbose:
         logging.info(pformat(quote.to_dict()))
 
     sys.exit(0)
```

### Comparing `intel_sgx_ra-2.0a2/src/intel_sgx_ra/error.py` & `intel_sgx_ra-2.0a3/src/intel_sgx_ra/error.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """intel_sgx_ra.error module."""
 
 
 class SGXQuoteNotFound(Exception):
     """SGX Quote extension not found in X509 certificate."""
 
 
+class SGXVerificationError(Exception):
+    """Error occured while verifying properties of SGX enclave."""
+
+
 class RATLSVerificationError(Exception):
-    """Cert public key different from report_data in SGX quote."""
+    """Certificate's public key different from report_data in SGX quote."""
 
 
 class SGXDebugModeError(Exception):
     """SGX enclave is in debug mode."""
 
 
 class CertificateRevokedError(Exception):
-    """Intel Root CA revoked."""
+    """Certificate has been revoked."""
 
 
 class PCCSResponseError(Exception):
     """Intel PCCS API reponse error."""
 
 
 class CommandNotFound(Exception):
```

### Comparing `intel_sgx_ra-2.0a2/src/intel_sgx_ra/pccs.py` & `intel_sgx_ra-2.0a3/src/intel_sgx_ra/pccs.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,43 +12,43 @@
     load_pem_x509_certificate,
 )
 
 from intel_sgx_ra.error import PCCSResponseError
 from intel_sgx_ra.quote import RE_CERT
 
 
-def get_crl_by_uri(base_url: str, uri: str) -> bytes:
+def get_crl_by_uri(pccs_url: str, uri: str) -> bytes:
     """Retrieve CRL by URI."""
     response = requests.get(
-        url=f"{base_url}/sgx/certification/v3/crl", json={"uri": uri}, timeout=30
+        url=f"{pccs_url}/sgx/certification/v4/crl", json={"uri": uri}, timeout=30
     )
 
     return response.content
 
 
-def get_root_ca_crl(base_url: str) -> CertificateRevocationList:
+def get_root_ca_crl(pccs_url: str) -> CertificateRevocationList:
     """Retrieve Root CA CRL."""
     response = requests.get(
-        url=f"{base_url}/sgx/certification/v3/rootcacrl", timeout=30
+        url=f"{pccs_url}/sgx/certification/v4/rootcacrl", timeout=30
     )
 
     return load_der_x509_crl(bytes.fromhex(response.text))
 
 
 def get_pck_certificate(
-    base_url: str,
+    pccs_url: str,
     encrypted_ppid: Optional[str],
     cpusvn: str,
     pcesvn: str,
     pceid: str,
     qeid: str,
 ) -> str:
     """Retrieve PCK Certificate from parameters."""
     response = requests.get(
-        url=f"{base_url}/sgx/certification/v3/pckcert",
+        url=f"{pccs_url}/sgx/certification/v4/pckcert",
         params={
             "encrypted_ppid": encrypted_ppid,
             "cpusvn": cpusvn,
             "pcesvn": pcesvn,
             "pceid": pceid,
             "qeid": qeid,
         },
@@ -57,32 +57,32 @@
 
     pck_cert = response.text
 
     return pck_cert
 
 
 def get_pck_cert_crl(
-    base_url: str, ca: Literal["processor", "platform"]
+    pccs_url: str, ca: Literal["processor", "platform"]
 ) -> CertificateRevocationList:
     """Retrieve PCK CRL."""
     response = requests.get(
-        url=f"{base_url}/sgx/certification/v3/pckcrl",
+        url=f"{pccs_url}/sgx/certification/v4/pckcrl",
         params={"ca": ca, "encoding": "der"},
         timeout=30,
     )
 
     return load_der_x509_crl(response.content)
 
 
 def get_tcbinfo(
-    base_url: str, fmscp: str
+    pccs_url: str, fmscp: str
 ) -> Tuple[Tuple[Certificate, Certificate], Dict[str, Any]]:
     """Retrieve TCB info from `fmscp`."""
     response = requests.get(
-        url=f"{base_url}/sgx/certification/v3/tcb", params={"fmspc": fmscp}, timeout=30
+        url=f"{pccs_url}/sgx/certification/v4/tcb", params={"fmspc": fmscp}, timeout=30
     )
     cert_chain = unquote(response.headers["SGX-TCB-Info-Issuer-Chain"])
     tcb_cert, root_ca_cert, *others = [
         load_pem_x509_certificate(raw_cert)
         for raw_cert in re.findall(RE_CERT, cert_chain.encode("utf-8"))
     ]
 
@@ -91,19 +91,19 @@
             "More than 2 certifices in header SGX-TCB-Info-Issuer-Chain"
         )
 
     return (tcb_cert, root_ca_cert), response.json()
 
 
 def get_qe_identity(
-    base_url: str,
+    pccs_url: str,
 ) -> Tuple[Tuple[Certificate, Certificate], Dict[str, Any]]:
     """Retrieve Quoting Enclave Identity."""
     response = requests.get(
-        url=f"{base_url}/sgx/certification/v3/qe/identity", timeout=30
+        url=f"{pccs_url}/sgx/certification/v4/qe/identity", timeout=30
     )
 
     cert_chain = unquote(response.headers["SGX-Enclave-Identity-Issuer-Chain"])
     tcb_cert, root_ca_cert, *others = [
         load_pem_x509_certificate(raw_cert)
         for raw_cert in re.findall(RE_CERT, cert_chain.encode("utf-8"))
     ]
@@ -112,19 +112,19 @@
             "More than 2 certifices in header SGX-Enclave-Identity-Issuer-Chain"
         )
 
     return (tcb_cert, root_ca_cert), response.json()
 
 
 def get_qve_identity(
-    base_url: str,
+    pccs_url: str,
 ) -> Tuple[Tuple[Certificate, Certificate], Dict[str, Any]]:
     """Retrieve Quoting Verification Enclave Identity."""
     response = requests.get(
-        url=f"{base_url}/sgx/certification/v3/qve/identity", timeout=30
+        url=f"{pccs_url}/sgx/certification/v4/qve/identity", timeout=30
     )
 
     cert_chain = unquote(response.headers["SGX-Enclave-Identity-Issuer-Chain"])
     tcb_cert, root_ca_cert, *others = [
         load_pem_x509_certificate(raw_cert)
         for raw_cert in re.findall(RE_CERT, cert_chain.encode("utf-8"))
     ]
```

### Comparing `intel_sgx_ra-2.0a2/src/intel_sgx_ra/quote.py` & `intel_sgx_ra-2.0a3/src/intel_sgx_ra/quote.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 SGX_QUOTE_MAX_SIZE: int = 8192
 
 RE_CERT: re.Pattern = re.compile(
     b"(-----BEGIN CERTIFICATE-----\n.*?\n-----END CERTIFICATE-----)", re.DOTALL
 )
 
-HEADER = struct.Struct(">HH4sHHI32s")
-REPORT_BODY = struct.Struct(">16sI12s16sQQ32s32s32s32s64sHHH42s16s64s")
+HEADER = struct.Struct("HH4sHHI32s")
+REPORT_BODY = struct.Struct("16sI12s16sQQ32s32s32s32s64sHHH42s16s64s")
 
 
 @dataclass
 class ReportBody:  # 384 bytes
     # pylint: disable=line-too-long
     """Representation of `sgx_report_body_t` structure (in `sgx_report.h`).
 
@@ -166,15 +166,15 @@
 
 @dataclass
 class AuthData:
     """SGX auth data."""
 
     signature: bytes  # 0
     public_key: bytes  # 64
-    qe_report: bytes  # 128
+    qe_report: ReportBody  # 128
     qe_report_signature: bytes  # 512
     qe_auth_data: bytes  # 576
     certification_data_type: int
     certification_data: bytes
 
     @classmethod
     def from_bytes(cls, raw_auth_data: bytes) -> "AuthData":
@@ -208,27 +208,27 @@
         offset += certification_data_len
 
         assert len(raw_auth_data) == offset
 
         return cls(
             signature,
             public_key,
-            qe_report,
+            ReportBody.from_bytes(qe_report),
             qe_report_signature,
             qe_auth_data,
             certification_data_type,
             certification_data,
         )
 
     def __bytes__(self) -> bytes:
         """Serialize AuthData."""
         return (
             self.signature
             + self.public_key
-            + self.qe_report
+            + bytes(self.qe_report)
             + self.qe_report_signature
             + len(self.qe_auth_data).to_bytes(2, byteorder="little")
             + self.qe_auth_data
             + self.certification_data_type.to_bytes(2, byteorder="little")
             + len(self.certification_data).to_bytes(4, byteorder="little")
             + self.certification_data
         )
```

### Comparing `intel_sgx_ra-2.0a2/src/intel_sgx_ra/ratls.py` & `intel_sgx_ra-2.0a3/src/intel_sgx_ra/ratls.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             cert = ssock.getpeercert(True)
             if not cert:
                 raise CertificateError("Can't get peer certificate")
             return ssl.DER_cert_to_PEM_cert(cert)
 
 
 def get_quote_from_cert(ratls_cert: Union[bytes, x509.Certificate]) -> Quote:
-    """Extract SGX quote from X509 certificate."""
+    """Extract SGX quote from X.509 certificate."""
     cert: x509.Certificate = (
         x509.load_pem_x509_certificate(ratls_cert)
         if isinstance(ratls_cert, bytes)
         else ratls_cert
     )
 
     try:
@@ -85,15 +85,15 @@
     except x509.extensions.ExtensionNotFound as exc:
         raise SGXQuoteNotFound from exc
 
     return Quote.from_bytes(quote_extension.value)
 
 
 def ratls_verify(ratls_cert: Union[str, bytes, Path, x509.Certificate]) -> Quote:
-    """Check user_report_data in SGX quote to match SHA256(cert.public_key())."""
+    """Compare `report_data` field in SGX quote with SHA256(ratls_cert.public_key())."""
     cert: x509.Certificate
 
     if isinstance(ratls_cert, bytes):
         cert = x509.load_pem_x509_certificate(ratls_cert)
     elif isinstance(ratls_cert, str):
         cert = x509.load_pem_x509_certificate(ratls_cert.encode("utf-8"))
     elif isinstance(ratls_cert, Path):
```

### Comparing `intel_sgx_ra-2.0a2/src/intel_sgx_ra/signer.py` & `intel_sgx_ra-2.0a3/src/intel_sgx_ra/signer.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a2/src/intel_sgx_ra.egg-info/PKG-INFO` & `intel_sgx_ra-2.0a3/src/intel_sgx_ra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intel-sgx-ra
-Version: 2.0a2
+Version: 2.0a3
 Summary: Intel SGX Remote Attestation verification library
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `intel_sgx_ra-2.0a2/src/intel_sgx_ra.egg-info/SOURCES.txt` & `intel_sgx_ra-2.0a3/src/intel_sgx_ra.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -17,9 +17,10 @@
 src/intel_sgx_ra.egg-info/entry_points.txt
 src/intel_sgx_ra.egg-info/not-zip-safe
 src/intel_sgx_ra.egg-info/requires.txt
 src/intel_sgx_ra.egg-info/top_level.txt
 src/intel_sgx_ra/cli/__init__.py
 src/intel_sgx_ra/cli/utils.py
 src/intel_sgx_ra/cli/verify.py
+tests/test_pccs.py
 tests/test_quote.py
 tests/test_regex.py
```

### Comparing `intel_sgx_ra-2.0a2/tests/test_quote.py` & `intel_sgx_ra-2.0a3/tests/test_quote.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 def test_quote_parsing(data_path):
     raw_quote: bytes = (data_path / "quote.dat").read_bytes()
     quote: Quote = Quote.from_bytes(raw_quote)
 
     assert quote
     assert bytes(quote) == raw_quote
     assert quote.report_body.mr_signer == bytes.fromhex(
-        "c1c161d0dd996e8a9847de67ea2c00226761f7715a2c422d3012ac10795a1ef5")
+        "ac2c9fa87e4c91768b1d0c47169466c50d5a98c790639fbaefe7352a59919980")
 
     pck_cert, pck_platform_ca_cert, root_ca_cert, *others = [
         x509.load_pem_x509_certificate(raw_cert)
         for raw_cert in quote.certs()
     ]
 
     assert not others  # only 3 certificates
 
 
 def test_quote_ra(data_path):
     raw_quote: bytes = (data_path / "quote.dat").read_bytes()
     quote: Quote = Quote.from_bytes(raw_quote)
 
-    verify_quote(quote, base_url="https://pccs.mse.cosmian.com")
+    verify_quote(quote, pccs_url="https://pccs.mse.cosmian.com")
```

### Comparing `intel_sgx_ra-2.0a2/tests/test_regex.py` & `intel_sgx_ra-2.0a3/tests/test_regex.py`

 * *Files identical despite different names*

