# Comparing `tmp/yubihsm-2.1.2.tar.gz` & `tmp/yubihsm-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yubihsm-2.1.2.tar", last modified: Mon Dec  5 09:23:53 2022, max compression
+gzip compressed data, was "yubihsm-2.1.3.tar", last modified: Wed May 17 07:22:24 2023, max compression
```

## Comparing `yubihsm-2.1.2.tar` & `yubihsm-2.1.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 dain      (1000) dain      (1000)        0 2022-12-05 09:23:53.494045 yubihsm-2.1.2/
--rw-r--r--   0 dain      (1000) dain      (1000)    11358 2018-11-26 08:28:32.000000 yubihsm-2.1.2/COPYING
--rw-r--r--   0 dain      (1000) dain      (1000)       64 2018-11-26 08:28:32.000000 yubihsm-2.1.2/MANIFEST.in
--rw-r--r--   0 dain      (1000) dain      (1000)      598 2022-12-05 09:23:53.495042 yubihsm-2.1.2/PKG-INFO
--rw-r--r--   0 dain      (1000) dain      (1000)     3556 2022-12-05 08:56:05.000000 yubihsm-2.1.2/README.adoc
--rw-r--r--   0 dain      (1000) dain      (1000)      118 2022-12-05 09:23:53.497039 yubihsm-2.1.2/setup.cfg
--rw-r--r--   0 dain      (1000) dain      (1000)     1604 2022-12-05 08:56:05.000000 yubihsm-2.1.2/setup.py
-drwxr-xr-x   0 dain      (1000) dain      (1000)        0 2022-12-05 09:23:53.365956 yubihsm-2.1.2/test/
--rw-r--r--   0 dain      (1000) dain      (1000)      578 2022-12-05 08:56:05.000000 yubihsm-2.1.2/test/__init__.py
-drwxr-xr-x   0 dain      (1000) dain      (1000)        0 2022-12-05 09:23:53.431130 yubihsm-2.1.2/test/device/
--rw-r--r--   0 dain      (1000) dain      (1000)      578 2022-12-05 08:56:05.000000 yubihsm-2.1.2/test/device/__init__.py
--rw-r--r--   0 dain      (1000) dain      (1000)     4163 2022-12-05 08:56:05.000000 yubihsm-2.1.2/test/device/test_attestation.py
--rw-r--r--   0 dain      (1000) dain      (1000)     5244 2022-12-05 08:56:05.000000 yubihsm-2.1.2/test/device/test_auth.py
--rw-r--r--   0 dain      (1000) dain      (1000)     5940 2022-12-05 08:56:05.000000 yubihsm-2.1.2/test/device/test_basic.py
--rw-r--r--   0 dain      (1000) dain      (1000)     3739 2022-12-05 08:56:05.000000 yubihsm-2.1.2/test/device/test_delete.py
--rw-r--r--   0 dain      (1000) dain      (1000)    22077 2022-12-05 08:56:05.000000 yubihsm-2.1.2/test/device/test_ec.py
--rw-r--r--   0 dain      (1000) dain      (1000)     8075 2022-12-05 08:56:05.000000 yubihsm-2.1.2/test/device/test_hmac.py
--rw-r--r--   0 dain      (1000) dain      (1000)     5412 2022-12-05 08:56:05.000000 yubihsm-2.1.2/test/device/test_logs.py
--rw-r--r--   0 dain      (1000) dain      (1000)     3294 2022-12-05 08:56:05.000000 yubihsm-2.1.2/test/device/test_opaque.py
--rw-r--r--   0 dain      (1000) dain      (1000)     6792 2022-12-05 08:56:05.000000 yubihsm-2.1.2/test/device/test_otp.py
--rw-r--r--   0 dain      (1000) dain      (1000)     2016 2022-12-05 08:56:05.000000 yubihsm-2.1.2/test/device/test_reset.py
--rw-r--r--   0 dain      (1000) dain      (1000)    23604 2022-12-05 08:56:05.000000 yubihsm-2.1.2/test/device/test_rsa.py
--rw-r--r--   0 dain      (1000) dain      (1000)    12240 2022-12-05 08:56:05.000000 yubihsm-2.1.2/test/device/test_wrap.py
--rw-r--r--   0 dain      (1000) dain      (1000)     2067 2022-12-05 08:56:05.000000 yubihsm-2.1.2/test/device/utils.py
--rw-r--r--   0 dain      (1000) dain      (1000)    13032 2022-12-05 08:56:05.000000 yubihsm-2.1.2/test/test_core.py
--rw-r--r--   0 dain      (1000) dain      (1000)     2179 2022-12-05 08:56:05.000000 yubihsm-2.1.2/test/test_defs.py
--rw-r--r--   0 dain      (1000) dain      (1000)     4302 2022-12-05 08:56:05.000000 yubihsm-2.1.2/test/test_objects.py
--rw-r--r--   0 dain      (1000) dain      (1000)     1808 2022-12-05 08:56:05.000000 yubihsm-2.1.2/test/test_utils.py
-drwxr-xr-x   0 dain      (1000) dain      (1000)        0 2022-12-05 09:23:53.458408 yubihsm-2.1.2/yubihsm/
--rw-r--r--   0 dain      (1000) dain      (1000)      949 2022-12-05 08:56:05.000000 yubihsm-2.1.2/yubihsm/__init__.py
-drwxr-xr-x   0 dain      (1000) dain      (1000)        0 2022-12-05 09:23:53.491053 yubihsm-2.1.2/yubihsm/backends/
--rw-r--r--   0 dain      (1000) dain      (1000)     1550 2022-12-05 08:56:05.000000 yubihsm-2.1.2/yubihsm/backends/__init__.py
--rw-r--r--   0 dain      (1000) dain      (1000)     2137 2022-12-05 08:56:05.000000 yubihsm-2.1.2/yubihsm/backends/http.py
--rw-r--r--   0 dain      (1000) dain      (1000)     2774 2022-12-05 08:56:05.000000 yubihsm-2.1.2/yubihsm/backends/usb.py
--rw-r--r--   0 dain      (1000) dain      (1000)    22276 2022-12-05 08:56:05.000000 yubihsm-2.1.2/yubihsm/core.py
--rw-r--r--   0 dain      (1000) dain      (1000)     8364 2022-12-05 08:56:05.000000 yubihsm-2.1.2/yubihsm/defs.py
--rw-r--r--   0 dain      (1000) dain      (1000)     3105 2022-12-05 08:56:05.000000 yubihsm-2.1.2/yubihsm/eddsa.py
--rw-r--r--   0 dain      (1000) dain      (1000)     1485 2022-12-05 08:56:05.000000 yubihsm-2.1.2/yubihsm/exceptions.py
--rw-r--r--   0 dain      (1000) dain      (1000)    40465 2022-12-05 08:56:05.000000 yubihsm-2.1.2/yubihsm/objects.py
--rw-r--r--   0 dain      (1000) dain      (1000)     1613 2022-12-05 08:56:05.000000 yubihsm-2.1.2/yubihsm/utils.py
-drwxr-xr-x   0 dain      (1000) dain      (1000)        0 2022-12-05 09:23:53.477090 yubihsm-2.1.2/yubihsm.egg-info/
--rwxr--r--   0 dain      (1000) dain      (1000)      598 2022-12-05 09:23:53.000000 yubihsm-2.1.2/yubihsm.egg-info/PKG-INFO
--rwxr--r--   0 dain      (1000) dain      (1000)      856 2022-12-05 09:23:53.000000 yubihsm-2.1.2/yubihsm.egg-info/SOURCES.txt
--rwxr--r--   0 dain      (1000) dain      (1000)        1 2022-12-05 09:23:53.000000 yubihsm-2.1.2/yubihsm.egg-info/dependency_links.txt
--rwxr--r--   0 dain      (1000) dain      (1000)       56 2022-12-05 09:23:53.000000 yubihsm-2.1.2/yubihsm.egg-info/requires.txt
--rwxr--r--   0 dain      (1000) dain      (1000)        8 2022-12-05 09:23:53.000000 yubihsm-2.1.2/yubihsm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:22:24.251028 yubihsm-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-17 07:22:15.000000 yubihsm-2.1.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-17 07:22:15.000000 yubihsm-2.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-17 07:22:24.251028 yubihsm-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-17 07:22:15.000000 yubihsm-2.1.3/README.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-17 07:22:24.251028 yubihsm-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-17 07:22:15.000000 yubihsm-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:22:24.247028 yubihsm-2.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-17 07:22:15.000000 yubihsm-2.1.3/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:22:24.247028 yubihsm-2.1.3/test/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-17 07:22:15.000000 yubihsm-2.1.3/test/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-17 07:22:15.000000 yubihsm-2.1.3/test/device/test_attestation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-17 07:22:15.000000 yubihsm-2.1.3/test/device/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-17 07:22:15.000000 yubihsm-2.1.3/test/device/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-17 07:22:15.000000 yubihsm-2.1.3/test/device/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22019 2023-05-17 07:22:15.000000 yubihsm-2.1.3/test/device/test_ec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-05-17 07:22:15.000000 yubihsm-2.1.3/test/device/test_hmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-17 07:22:15.000000 yubihsm-2.1.3/test/device/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-17 07:22:15.000000 yubihsm-2.1.3/test/device/test_opaque.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-17 07:22:15.000000 yubihsm-2.1.3/test/device/test_otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-17 07:22:15.000000 yubihsm-2.1.3/test/device/test_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23603 2023-05-17 07:22:15.000000 yubihsm-2.1.3/test/device/test_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-05-17 07:22:15.000000 yubihsm-2.1.3/test/device/test_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-17 07:22:15.000000 yubihsm-2.1.3/test/device/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-05-17 07:22:15.000000 yubihsm-2.1.3/test/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-17 07:22:15.000000 yubihsm-2.1.3/test/test_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-17 07:22:15.000000 yubihsm-2.1.3/test/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-17 07:22:15.000000 yubihsm-2.1.3/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:22:24.247028 yubihsm-2.1.3/yubihsm/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-17 07:22:15.000000 yubihsm-2.1.3/yubihsm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:22:24.251028 yubihsm-2.1.3/yubihsm/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-17 07:22:15.000000 yubihsm-2.1.3/yubihsm/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-17 07:22:15.000000 yubihsm-2.1.3/yubihsm/backends/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-17 07:22:15.000000 yubihsm-2.1.3/yubihsm/backends/usb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22276 2023-05-17 07:22:15.000000 yubihsm-2.1.3/yubihsm/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-05-17 07:22:15.000000 yubihsm-2.1.3/yubihsm/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-17 07:22:15.000000 yubihsm-2.1.3/yubihsm/eddsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-17 07:22:15.000000 yubihsm-2.1.3/yubihsm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40465 2023-05-17 07:22:15.000000 yubihsm-2.1.3/yubihsm/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-17 07:22:15.000000 yubihsm-2.1.3/yubihsm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:22:24.251028 yubihsm-2.1.3/yubihsm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-17 07:22:24.000000 yubihsm-2.1.3/yubihsm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-17 07:22:24.000000 yubihsm-2.1.3/yubihsm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 07:22:24.000000 yubihsm-2.1.3/yubihsm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-17 07:22:24.000000 yubihsm-2.1.3/yubihsm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 07:22:24.000000 yubihsm-2.1.3/yubihsm.egg-info/top_level.txt
```

### Comparing `yubihsm-2.1.2/COPYING` & `yubihsm-2.1.3/COPYING`

 * *Files identical despite different names*

### Comparing `yubihsm-2.1.2/PKG-INFO` & `yubihsm-2.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: yubihsm
-Version: 2.1.2
+Version: 2.1.3
 Summary: Python library for the YubiHSM 2
 Home-page: https://developers.yubico.com/YubiHSM2/
 Author: Yubico
 Author-email: yubico@yubico.com
-License: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: http
 Provides-Extra: usb
+License-File: COPYING
```

### Comparing `yubihsm-2.1.2/README.adoc` & `yubihsm-2.1.3/README.adoc`

 * *Files identical despite different names*

### Comparing `yubihsm-2.1.2/setup.py` & `yubihsm-2.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,11 +35,11 @@
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Topic :: Security :: Cryptography",
         "Topic :: Software Development :: Libraries",
     ],
     packages=find_packages(exclude=["test", "test.*"]),
     test_suite="test",
-    install_requires=["six", "cryptography>=1.8,<38"],
+    install_requires=["six", "cryptography>=2.2,<43"],
     extras_require={"http": ["requests"], "usb": ["pyusb"]},
     tests_require=["mock", "cryptography>=2.6"],
 )
```

### Comparing `yubihsm-2.1.2/test/__init__.py` & `yubihsm-2.1.3/test/__init__.py`

 * *Files identical despite different names*

### Comparing `yubihsm-2.1.2/test/device/__init__.py` & `yubihsm-2.1.3/test/device/__init__.py`

 * *Files identical despite different names*

### Comparing `yubihsm-2.1.2/test/device/test_attestation.py` & `yubihsm-2.1.3/test/device/test_attestation.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             private_key = rsa.generate_private_key(0x10001, 4096, default_backend())
         else:
             ec_curve = ALGORITHM.to_curve(algorithm)
             private_key = ec.generate_private_key(ec_curve, default_backend())
 
         builder = x509.CertificateBuilder()
         name = x509.Name(
-            [x509.NameAttribute(NameOID.COMMON_NAME, u"Test Attestation Certificate")]
+            [x509.NameAttribute(NameOID.COMMON_NAME, "Test Attestation Certificate")]
         )
         builder = builder.subject_name(name)
         builder = builder.issuer_name(name)
         one_day = datetime.timedelta(1, 0, 0)
         builder = builder.not_valid_before(datetime.datetime.today() - one_day)
         builder = builder.not_valid_after(datetime.datetime.today() + one_day)
         builder = builder.serial_number(int(uuid.uuid4()))
```

### Comparing `yubihsm-2.1.2/test/device/test_auth.py` & `yubihsm-2.1.3/test/device/test_auth.py`

 * *Files identical despite different names*

### Comparing `yubihsm-2.1.2/test/device/test_basic.py` & `yubihsm-2.1.3/test/device/test_basic.py`

 * *Files identical despite different names*

### Comparing `yubihsm-2.1.2/test/device/test_delete.py` & `yubihsm-2.1.3/test/device/test_delete.py`

 * *Files identical despite different names*

### Comparing `yubihsm-2.1.2/test/device/test_ec.py` & `yubihsm-2.1.3/test/device/test_ec.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import absolute_import, division
 
 from .utils import YubiHsmTestCase
 from yubihsm.defs import ALGORITHM, CAPABILITY, COMMAND, ERROR
-from yubihsm.defs import BRAINPOOLP256R1, BRAINPOOLP384R1, BRAINPOOLP512R1
 from yubihsm.utils import int_from_bytes
 from yubihsm.eddsa import load_ed25519_private_key, serialize_ed25519_public_key
 from yubihsm.objects import AsymmetricKey
 from yubihsm.exceptions import YubiHsmDeviceError
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, serialization
@@ -238,30 +237,30 @@
 
         resp = asymkey.derive_ecdh(ekey.public_key())
         self.assertEqual(secret, resp)
 
         asymkey.delete()
 
     def test_bp256r1_ecdsa_sign(self):
-        self.bp_r1_ecdsa_sign(BRAINPOOLP256R1(), hashes.SHA256())
+        self.bp_r1_ecdsa_sign(ec.BrainpoolP256R1(), hashes.SHA256())
 
     def test_bp384r1_ecdsa_sign(self):
-        self.bp_r1_ecdsa_sign(BRAINPOOLP384R1(), hashes.SHA384())
+        self.bp_r1_ecdsa_sign(ec.BrainpoolP384R1(), hashes.SHA384())
 
     def test_bp512r1_ecdsa_sign(self):
-        self.bp_r1_ecdsa_sign(BRAINPOOLP512R1(), hashes.SHA512())
+        self.bp_r1_ecdsa_sign(ec.BrainpoolP512R1(), hashes.SHA512())
 
     def test_bp256r1_derive_ecdh(self):
-        self.bp_r1_derive_ecdh(BRAINPOOLP256R1())
+        self.bp_r1_derive_ecdh(ec.BrainpoolP256R1())
 
     def test_bp384r1_derive_ecdh(self):
-        self.bp_r1_derive_ecdh(BRAINPOOLP384R1())
+        self.bp_r1_derive_ecdh(ec.BrainpoolP384R1())
 
     def test_bp512r1_derive_ecdh(self):
-        self.bp_r1_derive_ecdh(BRAINPOOLP512R1())
+        self.bp_r1_derive_ecdh(ec.BrainpoolP512R1())
 
 
 class TestBpR1(YubiHsmTestCase):
     def generate_bp_r1_sign(self, curve, hashtype):
         asymkey = AsymmetricKey.generate(
             self.session, 0, "Generate BP R1 Sign", 0xFFFF, CAPABILITY.SIGN_ECDSA, curve
         )
@@ -337,15 +336,14 @@
         asymkey.delete()
 
     def test_pubkey_p256(self):
         self.pubkey_p256(ec.SECP256R1())
 
 
 class TestEd25519(YubiHsmTestCase):
-
     vectors = [
         {
             "key": b"\x9d\x61\xb1\x9d\xef\xfd\x5a\x60\xba\x84\x4a\xf4\x92\xec\x2c\xc4\x44\x49\xc5\x69\x7b\x32\x69\x19\x70\x3b\xac\x03\x1c\xae\x7f\x60",  # noqa E501
             "pubkey": b"\xd7\x5a\x98\x01\x82\xb1\x0a\xb7\xd5\x4b\xfe\xd3\xc9\x64\x07\x3a\x0e\xe1\x72\xf3\xda\xa6\x23\x25\xaf\x02\x1a\x68\xf7\x07\x51\x1a",  # noqa E501
             "msg": b"",
             "sig": b"\xe5\x56\x43\x00\xc3\x60\xac\x72\x90\x86\xe2\xcc\x80\x6e\x82\x8a\x84\x87\x7f\x1e\xb8\xe5\xd9\x74\xd8\x73\xe0\x65\x22\x49\x01\x55\x5f\xb8\x82\x15\x90\xa3\x3b\xac\xc6\x1e\x39\x70\x1c\xf9\xb4\x6b\xd2\x5b\xf5\xf0\x59\x5b\xbe\x24\x65\x51\x41\x43\x8e\x7a\x10\x0b",  # noqa E501
         },
```

### Comparing `yubihsm-2.1.2/test/device/test_hmac.py` & `yubihsm-2.1.3/test/device/test_hmac.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from yubihsm.defs import ALGORITHM, CAPABILITY
 from yubihsm.objects import HmacKey
 import random
 import os
 
 
 class TestHmac(YubiHsmTestCase):
-
     vectors = [
         {
             "key": b"\x0b" * 20,
             "chal": b"Hi There",
             "exp_sha1": b"\xb6\x17\x31\x86\x55\x05\x72\x64\xe2\x8b\xc0\xb6\xfb\x37\x8c\x8e\xf1\x46\xbe\x00",  # noqa: E501
             "exp_sha256": b"\xb0\x34\x4c\x61\xd8\xdb\x38\x53\x5c\xa8\xaf\xce\xaf\x0b\xf1\x2b\x88\x1d\xc2\x00\xc9\x83\x3d\xa7\x26\xe9\x37\x6c\x2e\x32\xcf\xf7",  # noqa: E501
             "exp_sha512": b"\x87\xaa\x7c\xde\xa5\xef\x61\x9d\x4f\xf0\xb4\x24\x1a\x1d\x6c\xb0\x23\x79\xf4\xe2\xce\x4e\xc2\x78\x7a\xd0\xb3\x05\x45\xe1\x7c\xde\xda\xa8\x33\xb7\xd6\xb8\xa7\x02\x03\x8b\x27\x4e\xae\xa3\xf4\xe4\xbe\x9d\x91\x4e\xeb\x61\xf1\x70\x2e\x69\x6c\x20\x3a\x12\x68\x54",  # noqa: E501
```

### Comparing `yubihsm-2.1.2/test/device/test_logs.py` & `yubihsm-2.1.3/test/device/test_logs.py`

 * *Files identical despite different names*

### Comparing `yubihsm-2.1.2/test/device/test_opaque.py` & `yubihsm-2.1.3/test/device/test_opaque.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         self.assertEqual(len(self.session.get_pseudo_random(123)), 123)
 
     def test_certificate(self):
         private_key = ec.generate_private_key(
             ALGORITHM.EC_P256.to_curve(), default_backend()
         )
         name = x509.Name(
-            [x509.NameAttribute(x509.oid.NameOID.COMMON_NAME, u"Test Certificate")]
+            [x509.NameAttribute(x509.oid.NameOID.COMMON_NAME, "Test Certificate")]
         )
         one_day = datetime.timedelta(1, 0, 0)
         certificate = (
             x509.CertificateBuilder()
             .subject_name(name)
             .issuer_name(name)
             .not_valid_before(datetime.datetime.today() - one_day)
```

### Comparing `yubihsm-2.1.2/test/device/test_otp.py` & `yubihsm-2.1.3/test/device/test_otp.py`

 * *Files identical despite different names*

### Comparing `yubihsm-2.1.2/test/device/test_reset.py` & `yubihsm-2.1.3/test/device/test_reset.py`

 * *Files identical despite different names*

### Comparing `yubihsm-2.1.2/test/device/test_rsa.py` & `yubihsm-2.1.3/test/device/test_rsa.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,14 @@
     def test_pubkey_rsa(self):
         self.pubkey_rsa(2048)
         self.pubkey_rsa(3072)
         self.pubkey_rsa(4096)
 
 
 class TestOaep(YubiHsmTestCase):
-
     p = 0xECF5AECD1E5515FFFACBD75A2816C6EBF49018CDFB4638E185D66A7396B6F8090F8018C7FD95CC34B857DC17F0CC6516BB1346AB4D582CADAD7B4103352387B70338D084047C9D9539B6496204B3DD6EA442499207BEC01F964287FF6336C3984658336846F56E46861881C10233D2176BF15A5E96DDC780BC868AA77D3CE769  # noqa: E501
     q = 0xBC46C464FC6AC4CA783B0EB08A3C841B772F7E9B2F28BABD588AE885E1A0C61E4858A0FB25AC299990F35BE85164C259BA1175CDD7192707135184992B6C29B746DD0D2CABE142835F7D148CC161524B4A09946D48B828473F1CE76B6CB6886C345C03E05F41D51B5C3A90A3F24073C7D74A4FE25D9CF21C75960F3FC3863183  # noqa: E501
     d = 0x056B04216FE5F354AC77250A4B6B0C8525A85C59B0BD80C56450A22D5F438E596A333AA875E291DD43F48CB88B9D5FC0D499F9FCD1C397F9AFC070CD9E398C8D19E61DB7C7410A6B2675DFBF5D345B804D201ADD502D5CE2DFCB091CE9997BBEBE57306F383E4D588103F036F7E85D1934D152A323E4A8DB451D6F4A5B1B0F102CC150E02FEEE2B88DEA4AD4C1BACCB24D84072D14E1D24A6771F7408EE30564FB86D4393A34BCF0B788501D193303F13A2284B001F0F649EAF79328D4AC5C430AB4414920A9460ED1B7BC40EC653E876D09ABC509AE45B525190116A0C26101848298509C1C3BF3A483E7274054E15E97075036E989F60932807B5257751E79  # noqa: E501
     dp1 = 0xC73564571D00FB15D08A3DE9957A50915D7126E9442DACF42BC82E862E5673FF6A008ED4D2E374617DF89F17A160B43B7FDA9CB6B6B74218609815F7D45CA263C159AA32D272D127FAF4BC8CA2D77378E8AEB19B0AD7DA3CB3DE0AE7314980F62B6D4B0A875D1DF03C1BAE39CCD833EF6CD7E2D9528BF084D1F969E794E9F6C1  # noqa: E501
     dq1 = 0x2658B37F6DF9C1030BE1DB68117FA9D87E39EA2B693B7E6D3A2F70947413EEC6142E18FB8DFCB6AC545D7C86A0AD48F8457170F0EFB26BC48126C53EFD1D16920198DC2A1107DC282DB6A80CD3062360BA3FA13F70E4312FF1A6CD6B8FC4CD9C5C3DB17C6D6A57212F73AE29F619327BAD59B153858585BA4E28B60A62A45E49  # noqa: E501
     qinv = 0x6F38526B3925085534EF3E415A836EDE8B86158A2C7CBFECCB0BD834304FEC683BA8D4F479C433D43416E63269623CEA100776D85AFF401D3FFF610EE65411CE3B1363D63A9709EEDE42647CEA561493D54570A879C18682CD97710B96205EC31117D73B5F36223FADD6E8BA90DD7C0EE61D44E163251E20C7F66EB305117CB8  # noqa: E501
     e = 0x10001
```

### Comparing `yubihsm-2.1.2/test/device/test_wrap.py` & `yubihsm-2.1.3/test/device/test_wrap.py`

 * *Files identical despite different names*

### Comparing `yubihsm-2.1.2/test/device/utils.py` & `yubihsm-2.1.3/yubihsm/backends/usb.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,57 +8,75 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from __future__ import print_function, division
+from __future__ import absolute_import
 
-from yubihsm import YubiHsm
-from yubihsm.defs import BRAINPOOLP256R1, BRAINPOOLP384R1, BRAINPOOLP512R1
-from cryptography.hazmat.primitives.asymmetric import ec
-
-import unittest
-import time
-import os
-
-# Register Brainpool curves
-ec._CURVE_TYPES["brainpoolP256r1"] = BRAINPOOLP256R1
-ec._CURVE_TYPES["brainpoolP384r1"] = BRAINPOOLP384R1
-ec._CURVE_TYPES["brainpoolP512r1"] = BRAINPOOLP512R1
-
-
-DEFAULT_KEY = "password"
-
-
-@unittest.skipIf(os.environ.get("BACKEND", None) == "NONE", "Skipping device tests.")
-class YubiHsmTestCase(unittest.TestCase):
-    _HAS_RESET = False
-
-    def connect_hsm(self):
-        self.hsm = YubiHsm.connect(os.environ.get("BACKEND", None))
-        self.info = self.hsm.get_device_info()
-
-    def require_version(self, version, message=None):
-        if self.info.version < version:
-            m = "Requires version " + ".".join(map(str, version))
-            if message:
-                m += ": " + message
-            self.skipTest(m)
-
-    def setUp(self):
-        self.connect_hsm()
-        self.session = self.hsm.create_session_derived(1, DEFAULT_KEY)
-        if not YubiHsmTestCase._HAS_RESET:
-            print("RESETTING DEVICE!!!!")
-            self.session.reset_device()
-            YubiHsmTestCase._HAS_RESET = True
-            time.sleep(5)
-            self.setUp()
-
-    def tearDown(self):
-        self.session.close()
-        del self.session
-
-        self.hsm.close()
-        del self.hsm, self.info
+from ..exceptions import YubiHsmConnectionError
+import usb.core
+import usb.util
+
+
+YUBIHSM_VID = 0x1050
+YUBIHSM_PID = 0x0030
+
+
+class UsbBackend(object):
+    """A backend for communicating with a YubiHSM directly over USB."""
+
+    def __init__(self, serial=None):
+        """Construct a UsbBackend, connected to a YubiHSM via USB.
+
+        :param int serial: (optional) The serial number of the YubiHSM to
+            connect to.
+        """
+        for device in usb.core.find(
+            find_all=True, idVendor=YUBIHSM_VID, idProduct=YUBIHSM_PID
+        ):
+            if serial is None or int(device.serial_number) == serial:
+                break
+        else:
+            raise YubiHsmConnectionError("No YubiHSM found.")
+
+        try:
+            device.set_configuration()
+        except usb.core.USBError as e:
+            raise YubiHsmConnectionError(e)
+
+        # Flush any data waiting to be read
+        try:
+            device.read(0x81, 0xFFFF, 10)
+        except usb.core.USBError:
+            pass  # Errors here are expected, and ignored
+
+        self._device = device
+        self.timeout = 300
+
+    def transceive(self, msg):
+        """Send a verbatim message."""
+        try:
+            sent = self._device.write(0x01, msg, self.timeout * 1000)
+            if sent != len(msg):
+                raise YubiHsmConnectionError("Error sending data over USB.")
+            if sent % 64 == 0:
+                if self._device.write(0x01, b"", self.timeout * 1000) != 0:
+                    raise YubiHsmConnectionError("Error sending data over USB.")
+            return bytes(
+                bytearray(self._device.read(0x81, 0xFFFF, self.timeout * 1000))
+            )
+        except usb.core.USBError as e:
+            raise YubiHsmConnectionError(e)
+
+    def close(self):
+        usb.util.dispose_resources(self._device)
+
+    def __repr__(self):
+        v_int = self._device.bcdDevice
+        version = "{}.{}.{}".format((v_int >> 8) & 0xF, (v_int >> 4) & 0xF, v_int & 0xF)
+        return (
+            "{0.__class__.__name__}("
+            "version={1}, "
+            "serial={0._device.serial_number})"
+        ).format(self, version)
```

### Comparing `yubihsm-2.1.2/test/test_core.py` & `yubihsm-2.1.3/test/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,14 @@
         # function's signature
         hsm = YubiHsm(backend="")
         hsm.create_session_derived(auth_key_id, password)
 
         hsm.create_session.assert_called_once_with(auth_key_id, expect_enc, expect_mac)
 
     def test_get_device_info_mock_transceive(self):
-
         """
         Test get_device_info function by mocking the transceive function
         """
 
         backend = get_backend()
         backend.transceive = MagicMock(
             backend.transceive, return_value=_TRANSCEIVE_DEVICE_INFO
```

### Comparing `yubihsm-2.1.2/test/test_defs.py` & `yubihsm-2.1.3/test/test_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,33 +11,32 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import absolute_import, division
 
 from yubihsm.defs import ALGORITHM
-from yubihsm.defs import BRAINPOOLP256R1, BRAINPOOLP384R1, BRAINPOOLP512R1
 from cryptography.hazmat.primitives.asymmetric import ec
 
 import unittest
 
 
 class TestAlgorithm(unittest.TestCase):
     def test_to_curve(self):
         self.assertIsInstance(ALGORITHM.EC_P224.to_curve(), ec.SECP224R1)
         self.assertIsInstance(ALGORITHM.EC_P256.to_curve(), ec.SECP256R1)
         self.assertIsInstance(ALGORITHM.EC_P384.to_curve(), ec.SECP384R1)
         self.assertIsInstance(ALGORITHM.EC_P521.to_curve(), ec.SECP521R1)
         self.assertIsInstance(ALGORITHM.EC_K256.to_curve(), ec.SECP256K1)
-        self.assertIsInstance(ALGORITHM.EC_BP256.to_curve(), BRAINPOOLP256R1)
-        self.assertIsInstance(ALGORITHM.EC_BP384.to_curve(), BRAINPOOLP384R1)
-        self.assertIsInstance(ALGORITHM.EC_BP512.to_curve(), BRAINPOOLP512R1)
+        self.assertIsInstance(ALGORITHM.EC_BP256.to_curve(), ec.BrainpoolP256R1)
+        self.assertIsInstance(ALGORITHM.EC_BP384.to_curve(), ec.BrainpoolP384R1)
+        self.assertIsInstance(ALGORITHM.EC_BP512.to_curve(), ec.BrainpoolP512R1)
 
     def test_for_curve(self):
         self.assertEqual(ALGORITHM.for_curve(ec.SECP224R1()), ALGORITHM.EC_P224)
         self.assertEqual(ALGORITHM.for_curve(ec.SECP256R1()), ALGORITHM.EC_P256)
         self.assertEqual(ALGORITHM.for_curve(ec.SECP384R1()), ALGORITHM.EC_P384)
         self.assertEqual(ALGORITHM.for_curve(ec.SECP521R1()), ALGORITHM.EC_P521)
         self.assertEqual(ALGORITHM.for_curve(ec.SECP256K1()), ALGORITHM.EC_K256)
-        self.assertEqual(ALGORITHM.for_curve(BRAINPOOLP256R1()), ALGORITHM.EC_BP256)
-        self.assertEqual(ALGORITHM.for_curve(BRAINPOOLP384R1()), ALGORITHM.EC_BP384)
-        self.assertEqual(ALGORITHM.for_curve(BRAINPOOLP512R1()), ALGORITHM.EC_BP512)
+        self.assertEqual(ALGORITHM.for_curve(ec.BrainpoolP256R1()), ALGORITHM.EC_BP256)
+        self.assertEqual(ALGORITHM.for_curve(ec.BrainpoolP384R1()), ALGORITHM.EC_BP384)
+        self.assertEqual(ALGORITHM.for_curve(ec.BrainpoolP512R1()), ALGORITHM.EC_BP512)
```

### Comparing `yubihsm-2.1.2/test/test_objects.py` & `yubihsm-2.1.3/test/test_objects.py`

 * *Files identical despite different names*

### Comparing `yubihsm-2.1.2/test/test_utils.py` & `yubihsm-2.1.3/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `yubihsm-2.1.2/yubihsm/__init__.py` & `yubihsm-2.1.3/yubihsm/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 """
 
 
 from __future__ import absolute_import
 from .core import YubiHsm  # noqa F401
 
 
-__version__ = "2.1.2"
+__version__ = "2.1.3"
```

### Comparing `yubihsm-2.1.2/yubihsm/backends/__init__.py` & `yubihsm-2.1.3/yubihsm/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `yubihsm-2.1.2/yubihsm/backends/http.py` & `yubihsm-2.1.3/yubihsm/backends/http.py`

 * *Files identical despite different names*

### Comparing `yubihsm-2.1.2/yubihsm/core.py` & `yubihsm-2.1.3/yubihsm/core.py`

 * *Files identical despite different names*

### Comparing `yubihsm-2.1.2/yubihsm/defs.py` & `yubihsm-2.1.3/yubihsm/defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,47 +14,28 @@
 
 """Named constants used in YubiHSM commands."""
 
 
 from __future__ import absolute_import, division
 
 from cryptography.hazmat.primitives.asymmetric import ec
-from cryptography import utils
 from enum import IntEnum, unique
 import six
 
 
 if six.PY2:
     # Workaround for int max size on Python 2.
     from enum import Enum
 
     class _LongEnum(long, Enum):  # noqa F821
         """Like IntEnum, but supports larger values"""
 
     IntEnum = _LongEnum  # Use instead of IntEnum  # noqa F811
 
 
-@utils.register_interface(ec.EllipticCurve)
-class BRAINPOOLP256R1(object):
-    name = "brainpoolP256r1"
-    key_size = 256
-
-
-@utils.register_interface(ec.EllipticCurve)
-class BRAINPOOLP384R1(object):
-    name = "brainpoolP384r1"
-    key_size = 384
-
-
-@utils.register_interface(ec.EllipticCurve)
-class BRAINPOOLP512R1(object):
-    name = "brainpoolP512r1"
-    key_size = 512
-
-
 @unique
 class ERROR(IntEnum):
     """Error codes returned by the YubiHSM"""
 
     OK = 0x00
     INVALID_COMMAND = 0x01
     INVALID_DATA = 0x02
@@ -223,17 +204,17 @@
 
 _curve_table = {
     ALGORITHM.EC_P224: ec.SECP224R1,
     ALGORITHM.EC_P256: ec.SECP256R1,
     ALGORITHM.EC_P384: ec.SECP384R1,
     ALGORITHM.EC_P521: ec.SECP521R1,
     ALGORITHM.EC_K256: ec.SECP256K1,
-    ALGORITHM.EC_BP256: BRAINPOOLP256R1,
-    ALGORITHM.EC_BP384: BRAINPOOLP384R1,
-    ALGORITHM.EC_BP512: BRAINPOOLP512R1,
+    ALGORITHM.EC_BP256: ec.BrainpoolP256R1,
+    ALGORITHM.EC_BP384: ec.BrainpoolP384R1,
+    ALGORITHM.EC_BP512: ec.BrainpoolP512R1,
 }
 
 
 @unique
 class LIST_FILTER(IntEnum):
     """Keys for use to filter on in list_objects"""
```

### Comparing `yubihsm-2.1.2/yubihsm/eddsa.py` & `yubihsm-2.1.3/yubihsm/eddsa.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 
     def _serialize_ed25519_private_key(key):
         return key.private_bytes(Encoding.Raw, PrivateFormat.Raw, NoEncryption())
 
     def _deserialize_ed25519_public_key(raw_key):
         return ed25519.Ed25519PublicKey.from_public_bytes(raw_key)
 
-
 except (ImportError, UnsupportedAlgorithm):
 
     class _Ed25519PrivateKey(object):
         def __init__(self, private_bytes):
             self._private_bytes = private_bytes
 
     class _Ed25519PublicKey(object):
```

### Comparing `yubihsm-2.1.2/yubihsm/exceptions.py` & `yubihsm-2.1.3/yubihsm/exceptions.py`

 * *Files identical despite different names*

### Comparing `yubihsm-2.1.2/yubihsm/objects.py` & `yubihsm-2.1.3/yubihsm/objects.py`

 * *Files identical despite different names*

### Comparing `yubihsm-2.1.2/yubihsm/utils.py` & `yubihsm-2.1.3/yubihsm/utils.py`

 * *Files identical despite different names*

### Comparing `yubihsm-2.1.2/yubihsm.egg-info/PKG-INFO` & `yubihsm-2.1.3/yubihsm.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: yubihsm
-Version: 2.1.2
+Version: 2.1.3
 Summary: Python library for the YubiHSM 2
 Home-page: https://developers.yubico.com/YubiHSM2/
 Author: Yubico
 Author-email: yubico@yubico.com
-License: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: http
 Provides-Extra: usb
+License-File: COPYING
```

### Comparing `yubihsm-2.1.2/yubihsm.egg-info/SOURCES.txt` & `yubihsm-2.1.3/yubihsm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

